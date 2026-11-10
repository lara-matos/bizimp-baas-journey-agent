# Webhooks Pix

## Objetivo
Receber notificações assíncronas sobre o status da transação Pix.

## Fluxo recomendado
1. Receber o evento do webhook.
2. Validar assinatura e origem do provedor.
3. Confirmar o identificador da transação.
4. Consultar o status no sistema interno.
5. Atualizar o registro e disparar ações de follow-up.

## Boas práticas
- Verificar a assinatura HMAC ou mecanismo equivalente.
- Validar o payload antes de processar.
- Reprocessar eventos idempotentes com cuidado.
- Registrar falhas de validação para monitoramento.

## Status esperados
- `pending`
- `processing`
- `completed`
- `failed`
- `reversed`
