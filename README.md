# Projetos Power BI

Repositório com meus projetos de análise de dados e Business Intelligence em Power BI.

## Projetos

| Projeto | Descrição | Ferramentas |
| --- | --- | --- |
| [Análise de Campanhas de Marketing](#análise-de-campanhas-de-marketing) | Dashboard de 4 páginas sobre perfil, comportamento e resposta dos clientes às campanhas | Power BI, Power Query, DAX |

---

## Análise de Campanhas de Marketing

Projeto desenvolvido durante o curso **Microsoft Power BI para Business Intelligence e Data Science**, da Data Science Academy.

### Objetivo

Analisar uma base de clientes de uma empresa de varejo para entender **quem são os clientes, como eles gastam e como respondem às campanhas de marketing**, apoiando decisões de segmentação e de investimento em campanhas.

### Base de dados

- Arquivo CSV com mais de 25 variáveis por cliente: perfil (ano de nascimento, escolaridade, estado civil, salário anual, filhos e adolescentes em casa), gastos por categoria (alimentos, brinquedos, eletrônicos, móveis, utilidades e vestuário), canais de compra (loja, web e catálogo), visitas ao site, participação em campanhas e país.
- Os dados são do material do curso. [INSERIR aqui se o CSV está no repositório ou se deve ser baixado na plataforma do curso.]

### Estrutura do dashboard

| Página | O que mostra |
| --- | --- |
| **Visão Cliente** | Total de clientes, idade média e compras por canal (loja, web e catálogo); distribuição por escolaridade e estado civil; filtro por país |
| **Visão Comportamento** | Relação entre gasto total e salário anual (dispersão); gasto total por número de filhos e de adolescentes em casa; árvore de decomposição por escolaridade e estado civil |
| **Visão Campanhas** | Resultado das campanhas de marketing; salário anual por resultado; visitas ao site por perfil; efetividade da campanha por número de filhos |
| **Visão Pontos de Venda** | Gasto por categoria de produto em cada país; evolução do gasto total por ano e país |

### O que foi feito

- **Power Query:** importação do CSV, promoção de cabeçalhos e definição dos tipos de dados.
- **Coluna calculada (DAX):** `Idade`, calculada a partir do ano de nascimento.
- **Medida (DAX):** `TotalGasto1`, somando o gasto do cliente em todas as categorias e tratando valores vazios com `COALESCE`.
- **Visualizações:** cartões, colunas, dispersão, pizza, tabela dinâmica, gráfico de linhas e combinado, árvore de decomposição e segmentação por país.

### Principais conclusões

[INSERIR de 3 a 5 conclusões com números que você encontrou ao explorar o dashboard. Exemplos do formato:
- Clientes com [perfil X] tiveram gasto total [Y]% maior que [perfil Z].
- A categoria [X] concentrou [Y]% do gasto no país [Z].
- Clientes com [característica] responderam melhor às campanhas.]

### Telas

[INSERIR os prints. Salve as imagens na pasta `imagens/` e use o formato abaixo:]

```markdown
![Visão Cliente](imagens/visao-cliente.png)
![Visão Comportamento](imagens/visao-comportamento.png)
![Visão Campanhas](imagens/visao-campanhas.png)
![Visão Pontos de Venda](imagens/visao-pontos-de-venda.png)
```

### Como abrir

1. Baixe o arquivo `.pbix` deste repositório.
2. Abra no [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (gratuito, para Windows).
3. Se o Power BI não encontrar os dados, vá em **Transformar dados > Configurações da fonte de dados** e aponte para o CSV na sua máquina.

---

## Autor

**Alfonso Canfild** — [LinkedIn](https://linkedin.com/in/alfonso-canfild-54a974161) | [GitHub](https://github.com/AlfonsoCanfild)
