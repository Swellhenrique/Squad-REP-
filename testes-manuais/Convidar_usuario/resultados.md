# Resultados dos Testes – Convidar Usuário

**Sistema:** REP+ – Guarani Sistemas  
**Funcionalidade:** Convidar usuário  
**Tipo de teste:** Manual

## Objetivo

Avaliar o funcionamento da funcionalidade de convite de usuários, verificando o preenchimento dos campos obrigatórios, as validações de e-mail e o processamento dos convites.

## Execução dos testes

Foram definidos cenários positivos e negativos para avaliar os seguintes comportamentos:

- Envio de convite com informações válidas.
- Validação do tipo de usuário obrigatório.
- Validação do perfil de acesso obrigatório.
- Validação do preenchimento do e-mail.
- Tentativa de envio com endereço de e-mail inválido.
- Tratamento de e-mails já cadastrados no sistema.
- Tratamento de e-mails pertencentes a usuários inativos.
- Tratamento de e-mails que já receberam convites anteriormente.
- Processamento de convites válidos em conjunto com endereços que não podem receber novos convites.

## Registro dos resultados

Os resultados de cada caso de teste serão documentados considerando o comportamento esperado e o comportamento apresentado pelo sistema.

Para cada execução, serão atribuídos os seguintes status:

- **PASS:** comportamento apresentado conforme o esperado.
- **FAIL:** comportamento diferente do esperado.
- **BLOCKED:** impossibilidade de executar o teste devido a alguma condição impeditiva.

As evidências, incluindo capturas de tela e gravações, serão armazenadas na pasta `Evidencias`.

## Conclusão

A execução desses testes tem como finalidade verificar se o processo de convite funciona corretamente, garantindo que os campos obrigatórios sejam validados, que as regras de negócio relacionadas aos endereços de e-mail sejam respeitadas e que os convites permitidos sejam processados adequadamente.