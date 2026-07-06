# NineMoon — Privacy Policy / Policy das lojas (agora: redirect)

**Este repo não hospeda mais conteúdo jurídico.** Desde 2026-07-06, cada página aqui é um **stub de redirect** pro domínio próprio (`ninemoon.com.br`), onde o conteúdo (Política de Privacidade, Termos de Uso, Exclusão de Conta, Termos de Uso Profissional) vive de fato — repo `9moon-landing`.

> Contexto do ecossistema: [`../CLAUDE.md`](../CLAUDE.md).

---

## Por que ainda existe

O build **1.0.11** do app (já publicado nas lojas) tem as URLs `newprompt.github.io/ninemoon-privacy-policy/...` **hardcoded** em `sign_up_screen`, `privacy_security_screen` e `profile_screen`. Não dá pra mudar retroativo — então este domínio (GitHub Pages) **tem que continuar respondendo pra sempre**, redirecionando pro domínio novo. Não deletar o repo.

## O que tem aqui (stubs de redirect)

| Arquivo | Redireciona para |
|---|---|
| [`index.html`](index.html) | `https://ninemoon.com.br/privacidade` |
| [`9moon-privacy-policy.html`](9moon-privacy-policy.html) | `https://ninemoon.com.br/privacidade` |
| [`termos-de-uso.html`](termos-de-uso.html) | `https://ninemoon.com.br/termos` |
| [`excluir-conta.html`](excluir-conta.html) | `https://ninemoon.com.br/excluir-conta` |
| [`termos-profissional.html`](termos-profissional.html) | `https://ninemoon.com.br/termos-profissional` |

Cada stub tem: `<meta http-equiv="refresh">` (redirect imediato, funciona sem JS), `<link rel="canonical">` (SEO), `<script>location.replace(...)</script>` (redirect via JS, sem poluir o histórico do navegador) e um `<body>` mínimo com link "clique aqui" de fallback visível.

**Sem build, sem framework, sem dependências.** HTML autocontido, CSS inline mínimo.

## Regras

- **Não editar conteúdo jurídico aqui** — a fonte única agora é `9moon-landing` (`privacidade.html`, `termos.html`, `excluir-conta.html`, `termos-profissional.html`). Mudança de texto legal vai lá, não aqui.
- **Não apagar este repo nem os arquivos** — builds antigos do app dependem das URLs continuarem resolvendo.
- Se o domínio de destino (`ninemoon.com.br`) mudar de novo no futuro, atualizar as 5 URLs de redirect aqui.
- **Conventional Commits**; commit direto em `main` permitido (solo).
- Ver [`../docs/PLANO_MIGRACAO_PAGINAS_LEGAIS.md`](../docs/PLANO_MIGRACAO_PAGINAS_LEGAIS.md) pro histórico completo da migração.
