# Política de segurança

O Calls lida com conversas, voz e dados pessoais. Levamos relatos de vulnerabilidade a sério.

## Como relatar

> [!IMPORTANT]
> Não abra issue pública para falhas de segurança.

Use o **relato privado de vulnerabilidade** do GitHub no repositório afetado: aba **Security → Report a vulnerability**. Se não souber qual repositório é, relate em [`calls-site`](https://github.com/Calls-Comunicacoes/calls-site/security/advisories/new).

Inclua, se possível:

- o que é afetado (app, launcher, site, API ou servidor de voz) e a versão;
- passos para reproduzir ou uma prova de conceito;
- o impacto que você enxerga.

## O que esperar

| Etapa | Prazo |
|---|---|
| Confirmação de recebimento | até 3 dias úteis |
| Avaliação inicial e gravidade | até 7 dias úteis |
| Correção de falhas críticas | o quanto antes, com aviso a quem relatou |

Pedimos que a falha não seja divulgada antes da correção. Quem relatar de boa-fé recebe crédito no aviso de segurança, se quiser.

## Escopo

Dentro: app desktop, launcher, `calls.fbrdev.com.br`, `api.fbrdev.com.br`, `voz.fbrdev.com.br` e o código desta organização.

Fora: ataques de negação de serviço, engenharia social, spam e falhas em serviços de terceiros (Supabase, LiveKit, Mercado Pago, GitHub) que devem ser relatadas a eles.

## Versões com suporte

Durante a alpha, só a versão mais recente do canal `stable` recebe correções.
