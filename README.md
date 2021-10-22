# desafio_leo_qa
Repositório para realização de desafio LEO

História 1

Cenário: Validar realização de login

Objetivo: Verificar se o login é efetivado após preenchimento dos campos obrigatórios.

Pré-condições: 

1. Usuário cadastrado na plataforma com perfil de administrador.
2. Dados de acesso válidos, do usuário com perfil de administrador.
3. Desing da tela de login nas cores branco, azul e cinza.
4. Exibição de asterisco vermelho nos campos "Identificação de usuário" e "Senha'.
5. Exibição de checkbox "Lembrar identificação de usuário".

Passos:
1. Acessar a tela de login em: https://sandbox.moodledemo.net/login/index.php
2. Preencher o campo "Identificação de usuário" com dado correto;
3. Preencher o campo "Senha" com dado correto;
4. Habilitar checkbox "Lembrar identificação de usuário";
5. "Acessar".

Resultados esperados:

1. Tela de login exibe os campos "Identificação de usuário" e "Senha" vazios e sinalizados com asterisco na cor vermelha;
2. Ao "Acessar" o login do usuário "Administrador" deverá ser efetivado;
4. O usuário "Administrador" deverá ser redirecionado para a tela "Home".

Status: Reprovado

Bug identificado na tela de login.

Descrição:
Os campos "Identificação de usuário" e "Senha" não apresentam asteriscos na cor vermelha para indicação de obrigatoriedade de preenchimento.

Passos:
1. Acessar a tela de login em: https://sandbox.moodledemo.net/login/index.php

Evidência:
![image](https://user-images.githubusercontent.com/92929747/138388618-bab44676-b05d-4b05-89a0-a04a276f4589.png)


História 1 - Cenário alternativo 01

Cenário: Validar exibição de mensagem de login incorreto.

Objetivo: Verificar se mensagem de login incorreto é exibida após preenchimento dos campos com dados inválidos.

Pré-condições:

1. O usuário deverá estar cadastrado na plataforma com papel de administrador.
2. O usuário com papel de administrador deverá dispor de dados de acesso inválidos.

Passos:
1. Acessar a tela de login: https://sandbox.moodledemo.net/login/index.php
2. Preencher o campo "Identificação de usuário" com dado inválido.
3. Preencher o campo "Senha" com dado inválido.
4. "Acessar".

Resultados esperados:

1. Tela de login exibe os campos "Identificação de usuário" e "Senha" vazios;
2. Ao "Acessar" com os dados inválidos, a página deverá ser recarregada;
3. Os campos "Identificação de usuário" e "Senha" devem retornar vazios;
4. Deverá ser exibida a mensagem "Nome de usuário ou senha errados. Por favor tente outra vez".

Status: Aprovado

Evidência:
![image](https://user-images.githubusercontent.com/92929747/138390603-e39d9d96-4978-4223-aa55-ec400f6f6217.png)


História 1 - BDD

Cenário: 

DADO que estou na página de login

E possuo perfil de "Administrador" cadastrado na plataforma

E possuo dados de acesso corretos

QUANDO preencho os campos "Identificação de usuário" e "Senha"

E realizo o acesso

ENTÃO sou redirecionado para a tela "Home" da minha conta.




História 2

Cenário: Validar criação de curso fake

Objetivo: Verificar se curso é criado após preenchimento dos campos obrigatórios.

Pré-condições: 

1. Usuário cadastrado na plataforma com perfil de administrador;
2. Dados de acesso válidos, do usuário com perfil de administrador;
3. Exibição do menu "Administração do site" na página "Home";
4. Exibição da aba "Cursos" no menu "Administração do site";
5. Exibição de opção para adicionar novo curso na aba "Cursos";
6. Exibição de exclamações com fundo vermelho nos campos obrigatórios de cadastro do curso;
7. O campo "Número de identificação do curso" deve aceitar apenas números;

Passos:
1. Acessar a tela de login em: https://sandbox.moodledemo.net/login/index.php
2. Preencher o campo "Identificação de usuário" com dado correto;
3. Preencher o campo "Senha" com dado correto;
4. "Acessar";
5. No menu "Administração do site" clicar na aba "Cursos";
6. Na aba "Cursos" clicar na opção "Adicionar novo curso";
7. No campo "Nome completo do curso" preencher com "Curso Fake";
8. No campo "Nome pequeno do curso" preencher com "Curso Fake";
9. No campo "Número de identificação do curso" preencher com "01";
10. "Salvar e mostrar".

Resultados esperados:

1. Tela de login exibe os campos "Identificação de usuário" e "Senha" vazios;
2. Ao "Acessar" o login do usuário "Administrador" deverá ser efetivado;
4. Usuário "Administrador" deverá ser redirecionado para a tela "Home";
5. Na tela "Home" o "Administrador" conseguirá navegar no menu "Administração do site" > aba "Cursos" > "Adicionar novo curso";
6. Tela de cadastro do curso deverá ser exibida com os campos vazios;
7. Os campos "Nome completo do curso" e "Nome breve do curso" devem estar sinalizados com exclamações de fundo vermelho;
8. O campo "Número de identificação do curso" só deve aceitar valores numéricos no momento de seu preenchimento;
9. Ao "Salvar e mostrar" o "Administrador" deverá ser redirecionado para a página do curso criado.

Status: Aprovado



História 2 - cenário alternativo 02

Cenário: Validar criação de curso fake

Objetivo: Verificar se curso é criado após preenchimento dos campos obrigatórios.

Pré-condições: 

1. Usuário cadastrado na plataforma com perfil de administrador;
2. Dados de acesso válidos, do usuário com perfil de administrador;
3. Exibição do menu "Administração do site" na página "Home";
4. Exibição da aba "Cursos" no menu "Administração do site";
5. Exibição de opção para adicionar novo curso na aba "Cursos";
6. Exibição de exclamações com fundo vermelho nos campos obrigatórios de cadastro do curso;
7. O campo "Número de identificação do curso" deve aceitar apenas números;

Passos:
1. Acessar a tela de login em: https://sandbox.moodledemo.net/login/index.php
2. Preencher o campo "Identificação de usuário" com dado correto;
3. Preencher o campo "Senha" com dado correto;
4. "Acessar";
5. No menu "Administração do site" clicar na aba "Cursos";
6. Na aba "Cursos" clicar na opção "Adicionar novo curso";
7. No campo "Nome completo do curso" preencher com "Curso Fake";
8. No campo "Nome pequeno do curso" preencher com "Curso Fake";
9. No campo "Número de identificação do curso" preencher com "01fake";
10. "Salvar e mostrar".

Resultados esperados:

1. Tela de login exibe os campos "Identificação de usuário" e "Senha" vazios;
2. Ao "Acessar" o login do usuário "Administrador" deverá ser efetivado;
4. Usuário "Administrador" deverá ser redirecionado para a tela "Home";
5. Na tela "Home" o "Administrador" conseguirá navegar no menu "Administração do site" > aba "Cursos" > "Adicionar novo curso";
6. Tela de cadastro do curso deverá ser exibida com os campos vazios;
7. Os campos "Nome completo do curso" e "Nome breve do curso" devem estar sinalizados com exclamações de fundo vermelho;
8. O campo "Número de identificação do curso" só deve aceitar valores numéricos no momento de seu preenchimento;
9. Ao "Salvar e mostrar" o "Administrador" deverá ser redirecionado para a página do curso criado.

Status: Reprovado

Bug identificado na tela de cadastro do curso.

Descrição:
O campo "Número de identificação  do curso" aceitou o preenchimeto com letras.

Evidência:
![image](https://user-images.githubusercontent.com/92929747/138394868-f48711b0-860c-4445-9ef9-79cbdfca6614.png)




