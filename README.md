![image](https://github.com/FlavianaFXT/JS---Validando-Formularios/assets/113718720/b8eb4815-6e33-480a-adab-48db40646694)# JS---Validando-Formularios
curso Alura

Monica Hillman

No projeto deste curso, seremos uma dupla de pessoas desenvolvedoras que recebeu a tarefa de implementar validações nos campos do formulário de cadastro do Monibank.

Para isso acessaremos a [página do projeto](https://monicahillman.github.io/monibank/pages/abrir-conta-form.html) rodando em tempo real disponível neste link onde encontraremos as páginas de funcionamento da aplicação a fim de entender o que precisamos desenvolver. Na tela "Abrir conta" temos a primeira parte do formulário.

![image](https://github.com/FlavianaFXT/JS---Validando-Formularios/assets/113718720/f132979c-9f95-4a3e-abe9-2e19c0d5bfd6)


A parte superior central exibe uma imagem que representa a etapa 1 do formulário. Ela possui três círculos lado a lado na horizontal, conectados por uma linha que os atravessa, representando as três etapas do formulário. Da esquerda para a direita, temos um círculo na cor verde, enquanto que a linha e os dois círculos mais à direita estão preenchidos na cor cinza. Abaixo dessa imagem, ainda no eixo central, há o título "Preencha os campos abaixo para criar sua conta corrente!" em negrito. Abaixo deste temos seis campos com os títulos "Nome", "E-mail", "RG", "CPF" e "Data de Nascimento", seguidos de um checkbox clicável à esquerda da frase "Li e estou ciente quanto às condições de tratamento dos meus dados conforme descrito na Política de Privacidade do banco". Abaixo do checkbox existe um botão azul denominado "Avançar".
O campo "Nome" possui duas mensagens de verificação que são ativadas através das situações abaixo:

Se clicarmos no campo e em seguida clicarmos fora dele, a mensagem "O campo de nome não pode estar vazio." é exibida;
Se clicarmos no campo, e digitarmos alguns caracteres antes de clicarmos fora dele, a mensagem "Por favor, preencha um nome válido." será exibida.
Percebemos que o sistema possui várias mensagens customizadas para cada tipo de erro que pode ocorrer. Neste curso vamos implementá-las em todos os campos dessa página.

Em seguida, como bônus, implementaremos a página de reconhecimento facial do nosso formulário, disponível para consulta [neste link](https://monicahillman.github.io/monibank/pages/abrir-conta-form-2.html#). Nela a pessoa usuária será capaz de capturar uma imagem sua com a câmera — ou seja, aprenderemos a tirar fotografias com Javascript!

![image](https://github.com/FlavianaFXT/JS---Validando-Formularios/assets/113718720/4388b57a-cbc9-427a-baa9-5e8777a7a4b1)


 Ela exibe, na parte superior e centralizada, a mesma imagem que representa as três etapas do formulário, alterando suas cores. Agora temos dois círculos e metade da linha na cor verde, enquanto que a outra metade da linha e o círculo mais à direita estão preenchidos na cor cinza. Abaixo dessa imagem, ainda no eixo central, o título "Reconhecimento facial" é exibido em negrito, seguido logo abaixo pelo subtítulo "Clique no quadro abaixo para capturarmos uma imagem sua!". Abaixo deles existe um quadro retangular com um rosto sorridente que representa o espaço para a exibição da imagem capturada pela câmera.

Ao clicarmos no quadro será exibida a imagem da nossa câmera e um botão com o texto "Tirar foto". Se clicarmos no botão, a foto será tirada e ficará salva na tela. Abaixo da foto, será exibido um ícone de "check" (ou verificação) redondo junto à mensagem "Prontinho, imagem capturada!". Abaixo dessa mensagem será exibido um botão com o texto "Quero abrir minha conta!".

Para implementarmos tudo isso aprenderemos os dois seguintes tópicos:

Atributos do HTML5, como:

Required que torna o campo obrigatório;

Type que define o tipo de input;

min-length e max-length que controlam a quantidade de caracteres do input e

pattern que deve ser implementado no interior de regexs (expressões regulares, em português);

Ferramentas do Javascript, como:

addEventListener que detecta interações da pessoa usuária com o cadastro;

verificação de CPF que possuirá uma lógica para validar os seus dois últimos dígitos;

verificação de maioridade já que o Monibank não aceita menores de idade abrindo contas;

ValidityState para verificar os erros que ocorrem no preenchimento do elemento;

manipulação de DOM para imprimir mensagens de erro.

localStorage para salvar os dados. Mesmo que nosso formulário seja local, é necessário que suas informações sejam salvas em um local específico.

É importante que você já saiba:

Javascript assíncrono;
Manipulação de DOM;
localStorage;
um pouco de HTML e CSS, pois não construiremos essa parte no projeto — implementaremos códigos HTML e CSS já prontos.


Conhecer essas validações é essencial, pois podem ser aplicadas em qualquer aplicação que possua um formulário — seja para criação de contas em e-commerce e até mesmo em contas de redes sociais.

# PREPARANDO O AMBIENTE

VS Code
Live server
[Projeto Base](https://github.com/alura-cursos/monibank/tree/main)

# 1. VALIDANDO COM HTML

## Tipos de Input




