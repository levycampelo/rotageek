---
title: "Deploy automático com Netlify e GIT"
date: 2024-07-24T19:34:05-03:00
draft: true
authors:
  - levy
tags:
  - Blog Hugo
---
### Introdução
O Netlify é um serviço para hospedar sistemas que tem sua stack baseada em tecnologias front-end, que basicamente não precisam de banco de dados ou linguagens back-end para funcionar. O Netlify é grátis. Você só precisa se cadastrar e ser feliz.

O GitHub é uma plataforma de controle de versões gratuita que serve para gerir projetos e permite a colaboração entre uma grande comunidade de desenvolvedores.

### 1ª Adicionar o seu repositorio GIT no Netlify
A primeira parte é sincronizar o GIT com netlify, na tela principal da conta do netlify ir no botão "New site from GIT". Nessa parte você vai se autenticar com a conta do GIT e apontar qual repositório a conta do Netlify vai ter acesso. Além disso, você vai definir o comando que o Netlify deve executar o build do projeto. Nesse caso, usamos Hugo, o comando deve ser rodado com hugo -d.

![netlify](/build-netlify.png)

### 2ª Ajustar domain

Na conta do Netlify vem com um dominio default (xxx.netlify.app) caso você precise de um dominio próprio é possivel adquirir na plataforma ou fazer um CNAME através do registro.br por exemplo.

![dns](/dns.png)

### Finalizando
Após esse ajustes todas as alterações que você executar no seu codigo fonte e aplicar o git push, é trigado o Netlify e na sequencia ocorre o deploy.
