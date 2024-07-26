---
title: "O Que é Proxmox ?"
date: 2024-07-23T18:37:54-03:00
draft: true
authors:
  - levy
tags:
  - Virtualizacao 
---
Proxmox Virtual Environment é uma plataforma de código aberto para virtualização de servidores, permitindo a execução de máquinas virtuais (KVM) e containers (LXC) no mesmo ambiente. Este sistema operacional Linux facilita a criação e gestão de uma estrutura hiperconvergente.

Com o Proxmox, é possível dimensionar recursos de computação e armazenamento de forma escalável, desde um único nó até grandes clusters capazes de acomodar altas cargas de trabalho.

A plataforma oferece uma interface de gerenciamento baseada na web que integra ferramentas para configurar alta disponibilidade, armazenamento definido por software, rede e recuperação de desastres.

O Proxmox suporta praticamente qualquer configuração de hardware, desde pequenos servidores físicos até grandes soluções multiprocessadas conectadas a SANs.

### Principais Características do proxmox?
Virtualização de Máquinas e Containers: O Proxmox VE permite criar e gerenciar Máquinas Virtuais (VMs) usando QEMU e containers usando LXC.

Interface Web para Gerenciamento: Oferece uma interface web fácil de usar para a gestão completa do ambiente, eliminando a necessidade de linha de comando.

Alta Disponibilidade: Suporta a formação de clusters com alta disponibilidade, garantindo que serviços permaneçam ativos mesmo em caso de falha de um nó.

Armazenamento Distribuído: Compatível com diversas soluções de armazenamento, como Ceph, GlusterFS, ZFS, e outras opções locais e de rede.

Backup e Restauração: Possui ferramentas integradas para backup e recuperação de VMs e containers.

Firewall e Segurança: Inclui um firewall configurável por host, VM ou container.

Migração ao Vivo: Permite a migração ao vivo de VMs e containers, movendo-os sem interrupções entre hosts físicos.

API Aberta: Conta com uma API RESTful integrada para fácil gerenciamento e automação de tarefas.

![proxmox](/proxmox.png)
