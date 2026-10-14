# AGENTS.md

## Arquitetura
- Site estático. Todo o app está em `public/index.html` (CSS + JS inline, sem framework e sem build).
- `netlify.toml` publica `public/` sem comando de build.
- O estado (`S`) é salvo no `localStorage` com a chave `nutri_v1`. A escolha é do produto ("dados guardados só neste aparelho"): não acrescente backend sem que isso seja pedido.

## Convenções
- O código é compacto de propósito (identificadores curtos, uma função de render `rXxx` por aba, re-render via `innerHTML`). Mantenha esse estilo.
- As tabelas de referência (`NAF`, `OBJ`, `FAO`, `IMC`, `SEEDRAW`) ficam no topo do script e podem ser editadas ali.
- Escape todo texto vindo do usuário com `esc()` antes de inserir no HTML.
- Os valores nutricionais são por 100 g; as chaves dos nutrientes estão em `K`.
