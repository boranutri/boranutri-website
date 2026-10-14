# BORANutri

Aplicativo pessoal de nutrição em uma única página (pt-BR). Ele calcula a avaliação nutricional (IMC, TMB pela FAO/WHO/UNU 2004, GET e VET por objetivo), distribui os macronutrientes, mantém um diário alimentar por refeição a partir de um banco de alimentos (base TACO + alimentos personalizados), define metas, acompanha a evolução das medidas corporais e traz um guia ilustrado de como medir.

Todos os dados ficam no `localStorage` do navegador: nada é enviado a um servidor.

## Tecnologias
- HTML, CSS e JavaScript puros, sem dependências nem etapa de build
- Hospedagem estática no Netlify (`public/`)

## Rodar localmente
Abra `public/index.html` no navegador ou rode `netlify dev`.
