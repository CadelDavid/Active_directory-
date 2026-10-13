# Active_directory-
active directory , virtualization , hyper v , school project 

# Windows Server Infrastructure Project

## About the Project
This repository showcases the implementation and configuration of my final Windows Server Infrastructure project, developed for the Cybersecurity course at Instituto Superior de Tecnologias Avançadas (ISTEC). The primary goal was to design and deploy a secure, functional, and well-structured network infrastructure, applying core principles of system administration, network services, and access control.

## Network Topology
The architecture simulates a corporate environment featuring:
* **DC01:** Main Domain Controller processing authentications.
* **DC02:** Failover Domain Controller for redundancy.
* **DC03:** Remote Site Domain Controller.
* **GW01:** Gateway providing internet access.
* **PC01:** Client workstation.

## Key Features Implemented
* **Active Directory (AD DS):** Structured Organizational Units (OUs) and provisioned users and security groups segregated by departments (IT, HR, and Security).
* **Forest Trust Relationships:** Established a direct and two-way trust relationship between the domains `istec.pt` and `istec-net.pt`.
* **DNS & DHCP:** Configured DNS Forwarders (8.8.8.8 and 1.1.1.1) to resolve external queries and deployed DHCP for dynamic IP allocation to client machines.
* **File Server (SMB/NTFS):** Built a secure file-sharing structure with strict NTFS and network share permissions, ensuring that each department only accesses its respective data.
* **Group Policy Objects (GPOs):** Automated the mapping of network drives using *Item-Level Targeting*, deploying drives specifically based on the user's security group.

## Next Steps (Work in Progress)
* Implementation of File Screening and Quotas (FSRM).
* Windows Server Backup and File/System State restoration.
* High availability configurations using Hyper-V Replica and Live Migration between hosts.
* DHCP Failover and Conditional DNS Forwarders.

# Portugues 
# Projeto de Infraestrutura Windows Server

## Sobre o Projeto
Este repositório contém as evidências e configurações do meu projeto final de Infraestrutura Windows Server, desenvolvido para o curso de Cibersegurança no Instituto Superior de Tecnologias Avançadas (ISTEC). O objetivo principal foi desenhar e implementar uma infraestrutura de rede segura e funcional, aplicando princípios fundamentais de administração de sistemas, serviços de rede e controlo de acessos.

## Topologia da Rede
A arquitetura simula um ambiente corporativo com os seguintes componentes:
* **DC01:** Controlador de Domínio Principal (autenticação).
* **DC02:** Controlador de Domínio de Failover para redundância.
* **DC03:** Controlador de Domínio de instalação remota.
* **GW01:** Gateway para acesso à Internet.
* **PC01:** Máquina cliente da zona de utilizadores.

## Funcionalidades Implementadas
* **Active Directory (AD DS):** Criação de Unidades Organizacionais (OUs) estruturadas, bem como a gestão de utilizadores e grupos de segurança segregados por departamentos (TI, RH e Segurança).
* **Relação de Confiança (Trusts):** Configuração de uma confiança direta e bidirecional entre as florestas `istec.pt` e `istec-net.pt`.
* **DNS e DHCP:** Configuração de Forwarders no DNS (8.8.8.8 e 1.1.1.1) para resolução externa e implementação de servidor DHCP para atribuição dinâmica de IPs.
* **Servidor de Ficheiros (SMB/NTFS):** Criação de partilhas de rede com permissões NTFS rigorosas, garantindo o isolamento da informação e assegurando que cada departamento acede apenas aos seus dados.
* **Group Policy Objects (GPOs):** Mapeamento automático de unidades de rede em ambiente cliente através da funcionalidade *Item-Level Targeting*, validando o grupo de segurança do utilizador.

## Próximos Passos (Em desenvolvimento)
* Implementação de Quotas e File Screening (FSRM)
* Configuração de Windows Server Backup e restauro de ficheiros / System State.
* Alta disponibilidade com Hyper-V Replica e Live Migration de VMs entre hosts.
* Configuração de DHCP Failover e Conditional Forwarders no DNS.
