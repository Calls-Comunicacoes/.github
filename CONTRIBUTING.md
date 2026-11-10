# Como contribuir

Obrigado por ajudar a construir o Calls. Este guia vale para todos os repositórios da organização que não tenham um `CONTRIBUTING.md` próprio.

## Antes de começar

- Procure uma issue existente antes de abrir outra. Para bugs e ideias, use os modelos em **Issues → New issue**.
- Mudanças grandes (arquitetura, banco, fluxo de release) começam por uma issue ou ADR em `calls-docs`, não por um PR.
- Nunca suba segredos: chaves, tokens, `service_role`, `.env`. Use `.env.example` para documentar variáveis.

## Fluxo de trabalho

1. Crie uma branch a partir da `main`: `feat/nome-curto`, `fix/nome-curto`, `docs/nome-curto`.
2. Faça commits pequenos no padrão [Conventional Commits](https://www.conventionalcommits.org/pt-br/v1.0.0/):

   | Tipo | Quando usar |
   |---|---|
   | `feat` | Funcionalidade nova |
   | `fix` | Correção de bug |
   | `docs` | Só documentação |
   | `refactor` | Mudança interna sem alterar comportamento |
   | `test` | Testes |
   | `ci` / `chore` | Pipeline, dependências e manutenção |

3. Rode as checagens do repositório antes de abrir o PR (geralmente `pnpm typecheck` e os testes descritos no README).
4. Abra o PR preenchendo o modelo. Mudanças de interface levam print ou vídeo.
5. O merge acontece com CI verde e pelo menos uma revisão.

## Padrões

- **Idioma:** textos de interface, documentação e commits em português do Brasil. Nomes de código em inglês.
- **Sem emojis** em documentação, commits e textos do app.
- **Banco:** toda mudança de schema é uma migration nova em `calls-server/supabase/migrations`, com teste de RLS em pgTAP e o modelo de dados de `calls-docs` atualizado.
- **Design:** cores, tipografia e componentes vêm do `calls-design`. Não crie tokens soltos no app.

## Dúvidas

Abra uma issue com o rótulo `question` ou consulte o [planejamento](https://github.com/Calls-Comunicacoes/calls-docs/blob/main/PLANEJAMENTO.md) (acesso restrito a membros).
