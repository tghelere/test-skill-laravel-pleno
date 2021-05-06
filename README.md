## :rocket: Teste técnico para Desenvolvedor(a) Back-end Pleno na Ensinio

Este teste foi planejado para validar os conhecimentos necessários para a posição de Desenvolvedor(a) Back-end Pleno na Ensinio.

Serão avaliados aspectos relacionados aos conhecimentos em boas práticas de desenvolvimento, além dos conhecimentos nas tecnologias PHP, Laravel, e no seu ecosistema.

É esperado que você codifique com organização e siga os padrões determinados (estamos confiantes de que você pode vencer a vontade de fazer gambiarras :stuck_out_tongue_winking_eye:), e demonstre sua atenção em detalhes, capacidade de aprender e agregar valor.

Esperamos também que você se divirta e aprenda algo no processo. :blush:

## :eyes: O problema

- Desenvolver um CRUD de clientes, lojas e produtos que utilize as funcionalidades do **Laravel** descritas abaixo.
- O cenário das lojas deve receber informações de três respostas diferentes de APIs via pipeline (pipelines simulados nos arquivos .json presentes neste repositório) e, para solucionar o problema e armazenar as informações da loja em um só dado, é necessário abstrair os dados antes da entrada no banco de dados.

### Modelo do banco de dados das lojas
Coluna    | Valor  | Descrição
--------- | ------ | ------------------
id | BIGINT UNSIGNED NOT NULL AUTO_INCREMENT | Id único da Loja
name | VARCHAR(255) NOT NUL | Nome da loja
slug | VARCHAR(255) NOT NULL | Slug da loja - `UNIQUE INDEX `lojas` (`slug`)`
driver | VARCHAR(255) NOT NULL | Driver que irá receber as informações do pipeline - `UNIQUE INDEX `lojas` (`driver`)`
driver_meta | JSON NULL DEFAULT NULL | Informações salvas do driver
created_at | TIMESTAMP NULL DEFAULT NULL | Data de criação da loja
updated_at | TIMESTAMP NULL DEFAULT NULL | Data de atualização da loja

## :bulb: A proposta

Você deve codificar o projeto utilizando utilizando PHP Laravel. :smiley:

- Utilizar o _Laravel Breeze_ com _Inertia.js_ e enviar tudo configurado, login, reset de senha e as demais features do Laravel Breeze;
- Criar a API utilizando o _Laravel Sanctum_ e documentar com alguma ferramenta integrada;
- Abstrair a camada das lojas em diferentes drivers, explorando ao máximo as ferramentas do laravel para maximizar o desacoplamento das partes.

Por fim, forneça uma documentação, por meio de um arquivo "documentation.md", acerca do seu projeto. Inclua instruções completas para a execução da aplicação, e comentários que julgar pertinentes à avaliação.

## :dart: Requisitos do projeto

- O código deve seguir o padrão PSR adotado no PHP + Laravel;
- Organização do código;
- Criar seeders com factory do Laravel para popular o banco de dados;
- Fornecer uma documentação, incluindo instruções para a execução da sua aplicação.

## :clap: Diferenciais

- Aplicar cache;
- Escrever um ou mais testes :)

## :page_facing_up: Critérios de avaliação

- A qualidade do seu **código**;
- O cumprimento dos **requisitos**;
- A **estrutura** do seu projeto: esperamos ver componentização coesa, reuso, encapsulamento, separação de responsabilidades, etc;
- Seu **empenho**: não tem problema se algo não sair como desejado, mas tente! :blush:

## :email: Sobre a entrega

O teste tem até 7 dias para ser entregue a partir do recebimento das instruções.

Siga os passos abaixo:

- Clone este repositório;
- Crie uma branch com seu nome (no formato “nome-sobrenome”);
- Envie sua branch para este repositório em forma de PR;
- Envie o link da PR respondendo à **mesma conversa de email onde enviamos o link do desafio**.

Se por motivos de força maior não for possível cumprir com o prazo, por gentileza, nos informe respondendo à mesma conversa de email onde enviamos o link do desafio.
