---
title: "O que é Zabbix ?"
date: 2024-08-03T09:14:16-03:00
draft: true
authors:
  - levy
tags:
  - SRE
---
**Zabbix** é uma plataforma de monitoramento de código aberto projetada para rastrear a performance e disponibilidade de servidores, dispositivos de rede, aplicações e outros recursos de TI.

### Principais Funcionalidades do Zabbix:
**Coleta de Dados:** Zabbix coleta dados de diferentes fontes, como servidores, máquinas virtuais, dispositivos de rede, aplicações e muito mais. Ele utiliza agentes (Zabbix Agents) instalados nos dispositivos, SNMP (Simple Network Management Protocol) e outros métodos para coletar esses dados.

**Armazenamento de Dados:** Os dados coletados são armazenados em um banco de dados. O Zabbix é compatível com alguns tipos de bancos de dados, incluindo MySQL, SQLite, por exemplo.

**Visualização de Dados:** Zabbix fornece uma interface web intuitiva que permite aos usuários visualizar os dados de monitoramento em forma de gráficos, dashboards, mapas de rede e relatórios.

**Alertas e Notificações:** O sistema pode ser configurado para enviar alertas e notificações. As notificações podem ser enviadas por e-mail, ou Telegram.

**Automação:** Zabbix permite a automação de ações baseadas em eventos específicos. Por exemplo, se um servidor ficar inativo, o Zabbix pode automaticamente tentar reiniciá-lo ou executar um script.

### Como Funciona o Zabbix:
**Instalação do Servidor Zabbix:** A primeira parte é instalar o servidor Zabbix, que é a parte principal do sistema de monitoramento. Ele pode ser instalado em um servidor dedicado ou em uma máquina virtual.

**Configuração dos Agentes Zabbix:** Na sequencia, os agentes Zabbix são instalados nos dispositivos que você deseja monitorar. Esses agentes coletam dados de performance e disponibilidade e os enviam para o servidor Zabbix.

**Configuração dos Itens de Monitoramento:** No servidor Zabbix, você define os itens que deseja monitorar. Isso pode incluir métricas como uso de CPU, utilização de memória, tráfego de rede, tempo de resposta de aplicações, entre outros.

**Definição de Triggers:** Triggers são condições que definem quando um alerta deve ser gerado. Por exemplo, você pode configurar um trigger para enviar um alerta se o uso de Memória exceder 80% por mais de 5 minutos.

**Configuração de Ações:** Ações são respostas automáticas das triggers. Por exemplo, o Zabbix pode enviar uma mensagem para o Telegram quando um trigger for ativado.

### Benefícios do Uso do Zabbix:
**Monitoramento Centralizado:** Permite o monitoramento de toda a infraestrutura de TI a partir de um único ponto.

**RTO e ROP:** Identifica e responde rapidamente a problemas, reduzindo o tempo de inatividade e melhorando a disponibilidade dos serviços.

O Zabbix é amplamente utilizado em ambientes empresariais devido à sua robustez, flexibilidade e capacidade de monitorar uma ampla gama de dispositivos e aplicações.

![zabbix](/zabbix.png)
