# Critérios de Aceitação – Convidar Usuário

**Sistema:** REP+ – Guarani Sistemas  
**Funcionalidade:** Convidar usuário  
**Tipo de teste:** Manual

## CA001 – Convidar usuário com dados válidos

**Dado** que o usuário esteja autenticado no sistema REP+;

**E** acesse a funcionalidade de convite de usuários;

**Quando** selecionar um tipo de usuário válido;

**E** selecionar um perfil de acesso;

**E** informar um endereço de e-mail válido;

**E** confirmar o envio do convite;

**Então** o sistema deverá processar o convite;

**E** apresentar uma mensagem informando o resultado da operação.

## CA002 – Tipo de usuário não selecionado

**Dado** que o usuário esteja na tela de convite;

**Quando** deixar o campo de tipo de usuário sem seleção;

**Então** o botão de envio do convite deverá permanecer desabilitado.

## CA003 – Perfil de acesso não selecionado

**Dado** que o usuário esteja na tela de convite;

**Quando** deixar o campo de perfil de acesso sem seleção;

**Então** o botão de envio do convite deverá permanecer desabilitado.

## CA004 – E-mail não informado

**Dado** que o usuário esteja na tela de convite;

**Quando** deixar o campo de e-mail vazio;

**Então** o botão de envio do convite deverá permanecer desabilitado.

## CA005 – E-mail em formato inválido

**Dado** que o usuário tenha selecionado o tipo de usuário e o perfil de acesso;

**Quando** informar um endereço de e-mail em formato inválido;

**Então** o sistema deverá impedir o envio do convite;

**E** apresentar uma validação adequada.

## CA006 – Convite para e-mail já cadastrado ou convidado

**Dado** que exista um usuário cadastrado ou um convite pendente para determinado endereço de e-mail;

**Quando** tentar realizar um novo convite utilizando o mesmo endereço;

**Então** o sistema deverá aplicar a regra de negócio correspondente;

**E** informar o resultado da operação ao usuário.

## Regras gerais de aceitação

- O convite deve exigir o preenchimento dos três campos.
- O tipo de usuário deve ser selecionado.
- O perfil de acesso deve ser selecionado.
- O endereço de e-mail deve possuir formato válido.
- O botão de envio deve respeitar o preenchimento dos campos obrigatórios.
- O sistema deve informar o resultado do envio do convite.

**Observação:** Os comportamentos de duplicidade e validação de e-mail devem ser confirmados durante a execução dos testes e confrontados com as regras de negócio do REP+.