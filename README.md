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

Atualmente no meio virtual a forma mais comum de autenticação continua sendo o credenciamento baseado em senhas, e muitos pesquisadores continuam fazendo melhorias na segurança e na usuabilidade deste modelo [1], e por mais claro que estejam as inseguranças (esquecimento, repetição e mau elaboração de senhas por exemplo) deste método, é a maneira mais barata de se construir um sistema de segurança.

Gerenciadores de senhas resolvem grande parte do problema da autenticação por senhas, permitindo uma maior diversidade (senhas distintas para serviços distintos), e até mesmo aleatoriedade nas palavras-chave que as tornam imprevisíveis e, consequentemente, mais seguras.

Porém, assim como é mais barato para os sistemas em geral adotarem um credenciamento baseado em senhas, o mesmo acontece com os gerenciadores de senhas, que comumente pedem que o usuário crie uma senha mestra para acessar o sistema e poder coletar suas outras credenciais. A primeira vista parece uma boa troca, precisar lembrar de uma senha para não ter que lembrar das outras, porém esta única chave está sujeita aos problemas de outras senhas comuns; No cenário de um possível roubo do dispositivo enquanto a seção do sistema ainda está com as senhas desbloqueadas, a pessoa que estiver com o aparelho em mãos, terá acesso a todo o conteúdo sigiloso.

Dada a vulnerabilidade de uma senha mestra, o necessário se torna um método de autenticação que não precise de senha alguma, que seja anti-furto e que seja mais seguro do que os métodos tradicionais; Para isto o ideal, como segurido por estudantes da Universidade de Carleton [2], pode ser um gerenciador de senhas com dupla autenticação de dispositivos, isto é, para acessar o sistema pelo computador, o dono da conta deve possuír tanto seu computador quanto seu aparelho celular em mãos, ambos simultaneamente conectados, definindo uma seção enquanto os dois estão sincronizados.

Grandes sistemas já adotaram esta maneira de autenticação, como o Whatsapp Web [3], onde o usuário pareia seu aplicativo do Whatsapp no dispositivo móvel com o site, em um computador, através de um QR Code (podendo escolher se salva a seção no computador para não ter que parear das proximas vezes), e após feito isso, enquanto o celular estiver disponível, o usuário poderá continuar mexendo na versão Web do aplicativo, caso por qualquer motivo o celular perca a conexão, a seção é encerrada imediatamente.

### 1.1 Motivação
Grande parte dos gerenciadores de senhas atuais, por mais que tenham investido em fortes sistemas de criptografia para seus dados, optaram por adotar os métodos de autenticação mais baratos para proteger as senhas de seus usuários, os quais ficam vulneráveis a exposição em caso de roubo com uma seção do sistema aberta ou em um cenário onde a chave mestra é exposta a terceiros.

Existem sistemas de controle de senhas que possuem métodos de autenticação avançados e que oferece conforto a seus usuários, porém estes não são gratuítos e podém chegar a preços inacessíveis, sendo que a segurança das senhas de qualquer pessoa é crucial para o sigilo de suas mais sensiveis informações.

### 1.2 Objetivos
Este projeto visa proporcionar um software acessível para todo o público que necessita da segurança de suas informações, oferecendo um sistema de autenticação diferenciado e mais seguro do que os meios tradicionais podem oferecer.

A autenticação do usuário será feita utilizando dois dispositivos independentes pareados e conectados simultâneamente para que seja permitido para o usuário o acesso e a escrita de suas informações.

## Bibliografia

- [1] J. Bonneau, C. Herley, P. C. van Oorschot, and F. Stajano. The quest to replace passwords: a framework for comparative evaluation of web authentication schemes. In IEEE Symposium on Security and Privacy, 2012.
- [2] https://dl.acm.org/doi/10.1145/2420950.2420964
- [3] https://web.whatsapp.com/