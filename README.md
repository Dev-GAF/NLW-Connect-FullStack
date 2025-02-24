# Projeto - NLW Connect

NLW Connect é uma aplicação interativa que simula um sistema de inscrição e referência para um evento online. Desenvolvida com HTML, CSS e JavaScript, ela permite que usuários se inscrevam em um evento, gerem links únicos de referência e compartilhem com outras pessoas. À medida que outras pessoas se inscrevem através de seus links, os usuários acompanham as inscrições realizadas por suas referências.

### 🔗 Veja a página em funcionamento: https://dev-gaf.github.io/NLW-Connect-FullStack/

Este projeto é ideal para entender como criar uma dinâmica simples de referências e rastrear usuários sem a necessidade de um banco de dados, utilizando apenas armazenamento local no código.

## 🎯 Funcionalidades

* Cadastro de Usuários: Usuários podem se inscrever no evento fornecendo um e-mail e número de telefone.
* Link de Referência: Após o cadastro, cada usuário gera um link único que pode ser compartilhado.
* Acompanhamento de Referências: O número de inscrições feitas a partir do link do usuário é atualizado automaticamente.
* Sem Banco de Dados: Todos os dados dos usuários (como e-mail, telefone e referências) são armazenados localmente em um array no código.
* Interface Intuitiva: O projeto conta com uma interface simples e funcional, com elementos interativos para uma experiência de usuário agradável.

## ⚙ Tecnologias Utilizadas

* HTML: Estruturação da página e formulários de cadastro.
* CSS: Estilização da interface, criando um layout clean e responsivo.
* JavaScript: Lógica para o cadastro de usuários, geração de links de referência, e controle de estatísticas de inscrição.

## 👨‍💻 Estrutura de dados

Os dados de usuários são armazenados no seguinte formato:

![imagem alt](https://github.com/Dev-GAF/NLW-Connect-FullStack/blob/f322d126f84fff245c3e1eb7c89c0b852ae16550/Imagem.png)

* email: E-mail do usuário.
* phone: Número de telefone do usuário.
* ref: ID único de referência gerado para o usuário.
* refBy: ID do usuário que referenciou o novo usuário (caso haja uma referência).

## 📱 Inteface

A interface é composta por duas principais seções:

* Sobre o Evento: Informações gerais sobre o evento, incluindo data, horário e descrição.
* Formulário de Inscrição: Campo para inserir o e-mail e telefone, com o botão para confirmar a inscrição e gerar o link de referência.

Após a inscrição, o usuário verá o link gerado, podendo compartilhá-lo para gerar novas inscrições.

## 💡 Funcionalidades do Código

* Cadastro de Usuários: O código usa um formulário simples para capturar o e-mail e telefone. Se o usuário já existir, o sistema exibe a tela de convite com o link gerado.
* Referência e Compartilhamento: Quando o usuário compartilha seu link de referência, qualquer nova inscrição realizada com esse link é registrada e o número de inscrições é atualizado.
* Armazenamento Local: Todos os dados de inscrição são armazenados em um array dentro do código, sem necessidade de bancos de dados ou servidores.

### Código Principal

O código foi escrito para ser o mais simples e claro possível, com funções bem definidas:

* getUser(): Recupera um usuário pelo e-mail.
* getTotalSubscribers(): Retorna o número de inscrições feitas com o link de referência de um usuário.
* showInvite(): Exibe a tela de convite, mostrando o link gerado e o número de inscritos.
* saveUser(): Salva um novo usuário no array.
* formAction(): Captura os dados do formulário e realiza a inscrição ou exibe o link gerado.
* updateImageLinks(): Atualiza os links das imagens para garantir que elas sejam carregadas corretamente.

## 🎨 Design Responsivo

O projeto foi desenvolvido com CSS para garantir uma experiência agradável em diferentes dispositivos, como desktops, tablets e celulares.

## 🌱 Melhorias Futuras

* Validação de Formulários: Melhorar a validação dos campos de e-mail e telefone, garantindo um cadastro mais robusto.
* Estilização Avançada: Melhorar o design com animações e transições mais interativas, proporcionando uma experiência ainda mais fluida.

## 📄 Licença

### Este projeto está licenciado sob a MIT License. Consulte o arquivo LICENSE para mais detalhes.
