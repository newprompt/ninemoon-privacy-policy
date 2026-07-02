# NineMoon — Privacy Policy / Policy das lojas

Páginas **HTML estáticas** exigidas pelas lojas (App Store + Google Play) e pelo fluxo de exclusão de conta do app 9moon.

> Contexto do ecossistema: [`../CLAUDE.md`](../CLAUDE.md).

---

## O que tem aqui

- [`index.html`](index.html) — política de privacidade (página principal publicada — raiz do GitHub Pages).
- [`9moon-privacy-policy.html`](9moon-privacy-policy.html) — **cópia byte a byte** do `index.html` (URL nomeada usada nas fichas das lojas). ⚠ Toda edição em um vale para o outro — editar os dois e conferir com `diff index.html 9moon-privacy-policy.html` (deve retornar vazio).
- [`excluir-conta.html`](excluir-conta.html) — página de **exclusão de conta** (exigência da Google Play / Apple). Linkada do app e da ficha da loja.

**Sem build, sem framework, sem dependências.** HTML + CSS inline. Não há `package.json`, não há toolchain.

---

## Regras

- **Conteúdo jurídico** — alterar texto de política só com intenção clara. Não reescrever cláusula sem o dono pedir.
- **pt-BR**, tom formal, consistente entre as três páginas (nome do app, contato, datas).
- Ao mudar política, **atualizar a data de "última atualização"** na página.
- Mexeu no fluxo de exclusão de conta no app/backend? Conferir se `excluir-conta.html` continua coerente (passos, prazo, contato).
- Manter os arquivos **autocontidos** (CSS inline / mesma pasta) — devem abrir direto no navegador e em hospedagem estática simples.
- **Conventional Commits**; commit direto em `main` permitido (solo).
- Não introduzir tracker, script externo ou fonte remota sem necessidade — é página de privacidade, manter limpa.
