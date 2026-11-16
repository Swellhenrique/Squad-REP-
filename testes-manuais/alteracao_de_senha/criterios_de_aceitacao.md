# Critérios de Aceitação – Alteração de Senha
**Sistema:** REP+ – Guarani Sistemas  
**Funcionalidade:** Alteração de senha  
**Tipo de teste:** Manual

## CA001 – Alteração de senha com sucesso

**Dado** que o usuário esteja autenticado no sistema REP+;

**E** acesse a funcionalidade de alteração de senha;

**Quando** informar corretamente a senha atual;

**E** preencher a nova senha e a confirmação com valores iguais;

**E** confirmar a operação;

**Então** o sistema deverá atualizar a senha do usuário;

**E** apresentar uma mensagem informando que a alteração foi realizada com sucesso.

## CA002 – Senha atual incorreta

**Dado** que o usuário esteja na tela de alteração de senha;

**Quando** informar uma senha atual incorreta;

**E** tentar confirmar a operação;

**Então** o sistema deverá impedir a alteração da senha;

**E** apresentar uma mensagem informando que a senha atual está incorreta.

## CA003 – Confirmação de senha divergente

**Dado** que o usuário esteja na tela de alteração de senha;

**Quando** informar uma nova senha;

**E** preencher o campo de confirmação com um valor diferente;

**Então** o sistema deverá impedir a alteração;

**E** apresentar uma mensagem informando que as senhas não coincidem.

## CA004 – Campos obrigatórios não preenchidos

**Dado** que o usuário esteja na tela de alteração de senha;

**Quando** tentar realizar a operação sem preencher os campos obrigatórios;

**Então** o sistema deverá impedir a alteração;

**E** apresentar as validações necessárias para orientar o usuário.

## CA005 – Autenticação com a senha antiga após alteração

**Dado** que o usuário tenha realizado uma alteração de senha com sucesso;

**Quando** tentar acessar o sistema utilizando a senha anterior;

**Então** o sistema não deverá permitir a autenticação com a senha antiga.

## CA006 – Autenticação com a nova senha

**Dado** que o usuário tenha realizado uma alteração de senha com sucesso;

**Quando** tentar acessar o sistema utilizando a nova senha cadastrada;

**Então** o sistema deverá permitir a autenticação normalmente.

---

## Regras gerais de aceitação

- A alteração deve exigir a senha atual do usuário.
- A nova senha e sua confirmação devem ser iguais.
- Os campos obrigatórios devem ser validados.
- A senha anterior deve deixar de permitir autenticação após a alteração.
- A nova senha deve permitir autenticação após a alteração.
- O sistema deve apresentar mensagens claras sobre o resultado das operações.

**Observação:** Os critérios devem ser confrontados com o comportamento real do REP+ e com os requisitos definidos para a funcionalidade. Regras específicas de complexidade da senha não foram presumidas.