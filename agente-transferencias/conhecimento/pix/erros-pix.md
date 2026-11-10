# Erros Pix

## Erros frequentes
- Chave Pix inválida ou não encontrada.
- Valor fora do limite permitido.
- Conta ou instituição sem autorização para receber transferências.
- Falha de comunicação com a API de pagamentos.
- Requisição duplicada por timeout ou retry.

## Como tratar
- Registrar o código do erro e a mensagem detalhada.
- Repetir a operação somente quando houver garantia de idempotência.
- Retornar uma resposta clara ao cliente, sem expor dados sensíveis.
- Registrar logs com identificadores da transação.

## Exemplos de classificação
- `INVALID_KEY`
- `LIMIT_EXCEEDED`
- `UNAUTHORIZED_ACCOUNT`
- `BROKER_TIMEOUT`
- `DUPLICATE_TRANSACTION`
