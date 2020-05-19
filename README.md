# Trabalho de Graduação
FATEC Professor Jessen Vidal

Faculdade de Tecnologia de São José dos Campos

---

**Conceitos e fundamentos de segurança da informação aplicados no gerenciamento de senhas**

Author: [Fábio Romeiro](https://github.com/FabioRomeiro)

São José dos Campos - 2020

---

Orientador: Eduardo Sakaue

Coorientador: [Giuliano Araujo Bertoti](https://github.com/giulianobertoti)

---

## Resumo

---

## Abstract

---

## 1. Introdução

Atualmente no meio virtual a forma mais comum de autenticação continua sendo o credenciamento baseado em senhas, e muitos pesquisadores continuam fazendo melhorias na segurança e na usuabilidade deste modelo [1], e, como escrito por Daniel McCarney, da Universidade de Carleton, em seu estudo sobre design, implementação e avaliação de usuabilidade de gerenciadores de senhas [2], os gerenciadores de senhas resolvem grande parte dos problemas deste método de credenciamento, permitindo uma maior diversidade (senhas distintas para serviços distintos), e até mesmo aleatoriedade nas palavras-chave que as tornam imprevisíveis e, consequentemente, mais seguras.

Como destacado por Elizabeth Stobert, também da Universidade de Carleton, os problemas da autenticação por senha são conhecidos: Dificuldade de memorização de uma senha dificil, usuários possuindo um grande numero de senhas, e pessoas tenho diviculdade para acertar qual senha usar em qual conta [3]; Estes são os elementos chave que um gerenciador de senha foca resolver, normalmente definindo uma senha mestra, que é a responsável por dar acesso às outras senhas do usuário, porém assim como outras senhas, ela está sujeita a cair nos mesmos problemas de senhas normais.

Dada a vulnerabilidade de uma senha mestra, é interessante propor um gerenciador de senhas que não precise de senha alguma, que seja anti-furto e que possua um credenciamento mais rigoroso do que os métodos tradicionais; Como concluido por McCarney e outros quatro estudantes de Carleton [2], um sistema com dupla autenticação de dispositivos é um meio que diminuí a probabilidade de acesso das senhas por um infrator em caso de furto com a seção do gerenciador em aberto, isto é, para acessar o sistema pelo computador, o dono da conta deve possuír tanto seu computador quanto seu aparelho celular em mãos, ambos simultaneamente conectados, definindo uma seção enquanto os dois estão sincronizados.

Grandes sistemas já adotaram esta maneira de autenticação, como o Whatsapp Web [4], onde o usuário pareia seu aplicativo do Whatsapp no dispositivo móvel com o site, em um computador, através de um QR Code (podendo escolher se salva a seção no computador para não ter que parear das proximas vezes), e após feito isso, enquanto o celular estiver disponível, o usuário poderá continuar mexendo na versão Web do aplicativo, caso por qualquer motivo o celular perca a conexão, a seção é encerrada imediatamente.

### 1.1 Motivação
Os problemas mais comuns da autenticação de senhas como o grande número de senhas por usuários, dificuldade de memorização e dificuldade associar uma senha com uma conta em específico levam os usuários a decisões inseguras, como escolher senhas fáceis de lembrar, o que as tornam também faceis de decifrar por invasores, reutilizar senhas em multiplas contas, e escreve-las em algum lugar físico [3]; E um gerenciador de senhas consegue previnir que estes problemas venham a acontecer.

Já existem muitos sistemas de controle de senha no mercado, como o Dashlane, RoboForm, LasPass, Keeper e CyberArk, que investem bastante na criptografia do armazenamento de seus dados e na autenticação do usuário no sistema tomam medidas inocentes [1], não prevendo um dos principios chaves do gerenciador de senhas, esquecimento ou ma elaboração da senha mestra para o sistema, e não se preparando para um caso de furto enquanto a seção da aplicação está ativa.

### 1.2 Objetivos
Este projeto visa o desenvolvimento de um software onde os usuários poderão guardar e gerar senhas randomizadas e complexas para que a segurança de suas informações não seja dependente de sua memorização ou de um meio físico.

A autenticação do usuário para entrar neste gerenciador terá uma abordagem não tradicional, utilizando dois dispositivos independentes, pareados e conectados simultâneamente para que seja permitido para o usuário o acesso e a escrita de suas informações.

## Bibliografia

- [1] J. Bonneau, C. Herley, P. C. van Oorschot, and F. Stajano. The quest to replace passwords: a framework for comparative evaluation of web authentication schemes. In IEEE Symposium on Security and Privacy, 2012.
- [2] https://dl.acm.org/doi/10.1145/2420950.2420964
- [3] https://dl.acm.org/doi/pdf/10.1145/2683467.2683471
- [4] https://web.whatsapp.com/