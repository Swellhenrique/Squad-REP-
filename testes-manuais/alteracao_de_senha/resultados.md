# Resultados dos Testes – Alteração de Senha

**Sistema:** REP+ – Guarani Sistemas  
**Funcionalidade:** Alteração de senha  
**Tipo de teste:** Manual

## Objetivo

Avaliar o funcionamento da funcionalidade de alteração de senha, verificando se o sistema realiza a atualização corretamente e se as validações impedem operações com informações inválidas.

## Execução dos testes

Foram definidos cenários positivos e negativos para avaliar os seguintes comportamentos:

- Alteração de senha com informações válidas.
- Tentativa de autenticação utilizando a senha antiga.
- Autenticação utilizando a nova senha.
- Tentativa de alteração informando a senha atual incorretamente.
- Preenchimento de senhas divergentes.
- Tentativa de alteração com campos obrigatórios vazios.

## Registro dos resultados

Os resultados de cada caso de teste serão registrados considerando o comportamento esperado e o comportamento apresentado pelo sistema.

Para cada execução, serão atribuídos os seguintes status:

- **PASS:** comportamento apresentado conforme o esperado.
- **FAIL:** comportamento diferente do esperado.
- **BLOCKED:** impossibilidade de executar o teste devido a alguma condição impeditiva.

As evidências coletadas durante a execução serão armazenadas na pasta `Evidencias`.

## Conclusão

A execução desses testes tem como finalidade verificar a confiabilidade da funcionalidade de alteração de senha, garantindo que as atualizações sejam realizadas corretamente e que as validações previstas sejam respeitadas.