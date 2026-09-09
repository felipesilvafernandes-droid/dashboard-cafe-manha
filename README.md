# Dashboard · Custo & Descarte — Café da Manhã

Painel visual com os indicadores de custo, CMV e descarte do café da manhã, gerado a partir da planilha de contagem diária/mensal do operacional.

🔗 **Link publicado:** _adicione aqui a URL do GitHub Pages depois de ativado (Settings → Pages)_

## O que este painel mostra

- **Custo total do período** e **CMV** (custo ÷ receita de café da manhã)
- **Valor total descartado** e sua participação sobre o custo e sobre a receita
- **Top 10 itens** que mais geraram descarte, em R$
- **Descarte por categoria** (Padaria, Proteínas, Bebidas, Doces, Laticínios, Guarnições, Frutas)
- **Composição do atendimento** (hóspedes com café incluso vs. passantes)
- Demonstrativo completo com todos os itens descartados no período

## Fonte dos dados

O HTML é gerado a partir do arquivo Excel operacional (abas **CUSTO** e **DESCARTE**). Os números são apurados uma vez e "congelados" no HTML — ou seja, este arquivo é uma **foto** do período informado no cabeçalho da página, não um painel conectado ao vivo à planilha.

Para atualizar com dados de um novo período:
1. Gere/atualize a planilha Excel com as abas CUSTO e DESCARTE.
2. Recalcule os indicadores (custo total, descarte por item, CMV, categorias).
3. Substitua o `index.html` deste repositório pela nova versão e suba de novo (**Add file → Upload files → Commit changes**).
4. O GitHub Pages atualiza o link automaticamente em 1–2 minutos, sem precisar reconfigurar nada.

## Estrutura do repositório

```
index.html   → o dashboard (arquivo único, sem dependências externas além de fontes/gráficos via CDN)
README.md    → este arquivo
```

## Como visualizar localmente

Basta abrir o `index.html` em qualquer navegador — não precisa de servidor nem instalação.

## Próximos passos

Esta mesma base de dados (item, categoria, quantidade, preço, valor) está estruturada para alimentar um relatório em **Power BI**, reaproveitando os mesmos agrupamentos usados aqui no HTML.
