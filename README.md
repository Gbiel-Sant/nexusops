# NexusOps / DataGalaxy — Plataforma de Análise de Incidentes de TI

> Projeto do **FIAP Enterprise Challenge 2026** em parceria com a **Locaweb**, voltado à análise de padrões de incidentes de TI e, ao longo das sprints, à construção de uma plataforma de AIOps para monitoramento e previsão.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-EDA-150458)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626)
![Status](https://img.shields.io/badge/Status-Em_andamento_(Sprint_3_de_4)-orange)

---

## Status do projeto

**Em desenvolvimento — Sprint 3 de 4.** Este repositório evolui a cada sprint do challenge. Abaixo, o que já está entregue e o que está planejado.

### Concluído (Sprint 2)
- ✅ **Análise Exploratória de Dados (EDA)** dos incidentes de TI
- ✅ **Tratamento e organização dos dados**
- ✅ **Definição da arquitetura** da solução
- ✅ **Apresentação da Sprint 2** com achados e visualizações

### Em andamento / planejado (Sprints 3–4)
- 🔄 **BI / Dashboard** de acompanhamento (iniciado)
- ⏳ **Modelo de ML / AIOps** para análise preditiva de incidentes
- ⏳ **Deploy e infraestrutura** em nuvem (Azure Container Instances, FastAPI)

---

## Contexto de negócio

A Locaweb precisava entender **por que o volume de incidentes de TI crescia** e **onde os problemas se concentravam**, para direcionar esforços de mitigação de forma baseada em dados.

**Pergunta analítica central:** onde estão concentrados os incidentes, e o que explica o crescimento no volume ao longo do tempo?

---

## Principais achados (EDA — Sprint 2)

- **Concentração:** uma única equipe respondia por **~75% de todos os incidentes** registrados — o que redireciona completamente o foco da operação.
- **Causa do crescimento:** o aumento no volume **não** refletia piora no ambiente, e sim a implantação de um **pipeline de monitoramento automatizado** (jan/2025), que passou a capturar eventos antes invisíveis.
- **Implicação:** o "crescimento" era, na verdade, ganho de visibilidade — insight que evita conclusões erradas sobre degradação de serviço.

---

## Stack técnico

| Camada | Ferramentas | Status |
|---|---|---|
| Análise / EDA | Python, pandas | ✅ concluído |
| Visualização | matplotlib, seaborn | ✅ concluído |
| Ambiente | Jupyter Notebook | ✅ concluído |
| BI / Dashboard | Power BI | 🔄 iniciado |
| ML / AIOps | (planejado) | ⏳ Sprint 3–4 |
| Deploy | Azure Container Instances, FastAPI | ⏳ Sprint 3–4 |

---

## Metodologia (EDA)

1. **Coleta e limpeza** — tratamento de registros de incidentes, padronização de categorias e datas.
2. **EDA** — análise de distribuição por equipe, categoria e período; identificação de concentração e outliers.
3. **Análise temporal** — investigação do ponto de inflexão no volume e correlação com a mudança de monitoramento.
4. **Visualização** — gráficos de distribuição e séries temporais para comunicar os achados.
5. **Apresentação** — consolidação dos resultados em slides para a entrega da Sprint 2.

---

## Estrutura do repositório

\`\`\`
nexusops/
├── data/
│   └── incidentes_anonimizado.csv     # dados anonimizados (equipes mascaradas)
├── notebooks/
│   └── eda_incidentes.ipynb           # análise da Sprint 2
├── figures/
│   └── *.png                          # visualizações exportadas
├── docs/
│   └── arquitetura.md                 # definição de arquitetura
└── README.md
\`\`\`

---

## Como executar (EDA)

\`\`\`bash
git clone https://github.com/Gbiel-Sant/nexusops.git
cd nexusops
pip install -r requirements.txt
jupyter notebook notebooks/eda_incidentes.ipynb
\`\`\`

---

## Nota sobre os dados

Os dados foram **anonimizados** antes da publicação: nomes reais de equipes e identificadores sensíveis foram substituídos por rótulos genéricos (Team01, Team02, …), preservando a confidencialidade da empresa parceira.

---

## Autor

**Gabriel Santana Ferreira de Morais**
Analista de Dados & BI · [LinkedIn](https://www.linkedin.com/in/gabrielsantanadata) · [GitHub](https://github.com/Gbiel-Sant)

*Papel no projeto: responsável pela Análise Exploratória de Dados (EDA), visualizações e apresentação dos resultados (Sprint 2). Contribuindo nas etapas de BI e infraestrutura nas sprints seguintes.*
