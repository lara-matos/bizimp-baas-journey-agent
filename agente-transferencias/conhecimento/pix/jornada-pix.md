# Jornada PIX

## Visão geral
Este documento descreve o fluxo esperado para transferências via Pix em um agente de pagamentos.

## Etapas principais
1. Receber a solicitação de pagamento.
2. Validar dados do destinatário e valor.
3. Confirmar o tipo de chave Pix utilizada.
4. Executar a transação com a instituição emissora ou API integradora.
5. Registrar o resultado e emitir resposta ao cliente.

## Pontos de atenção
- Validar CPF/CNPJ, chave Pix, valor e horário da operação.
- Tratar idempotência para evitar duplicidade de pagamento.
- Monitorar status de confirmação e eventual timeout.

## Checklist operacional
- Chave Pix válida
- Valor positivo
- Dados do beneficiário confirmados
- Retorno da operação registrado
