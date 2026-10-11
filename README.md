# Miniguia de Estudos: IA Aplicada à Análise de Dados

Repositório de estudos do Bootcamp Power BI (Santander/DIO), com o desafio de projeto "Engenharia de Prompts e NotebookLM" — construção de um Caderno Temático usando IA como ferramenta de aprendizagem ativa.

## Acesso rápido

| Material | Onde encontrar |
| --- | --- |
| Miniguia completo em Markdown | [Ler o miniguia](./miniguia-ia-dados.md) |
| Manual em PDF | [Abrir o manual](./manual-ia-analise-dados.pdf) |
| Projetos práticos de Power BI | [Explorar os desafios](https://github.com/AdrianaOli-ve/DESAFIOSPWB) |

**Neste README:** [Contexto e objetivos](#1-contexto-e-objetivos) · [Fontes](#2-curadoria-de-fontes) · [Engenharia de prompts](#3-engenharia-de-prompts-e-cicatrizes) · [Miniguia](#4-miniguia-de-estudo-entrega-final) · [Materiais](#5-material-complementar)


---

## 1. Contexto e Objetivos

O assunto escolhido para este caderno temático foi **Inteligência Artificial aplicada à Análise de Dados**, com foco em compreender:
- os fundamentos e etapas do processo de análise de dados;
- como a IA (incluindo IA Generativa) se conecta a esse processo;
- riscos, limitações, vieses e boas práticas de uso ético e seguro de IA, com base nos frameworks da UNESCO e do NIST.

**Objetivos de estudo:**
- Consolidar o entendimento sobre análise de dados, Machine Learning e IA Generativa;
- Praticar engenharia de prompts de forma estruturada e crítica, documentando acertos e dificuldades;
- Produzir um material de consulta rápida (miniguia) para revisões futuras.

---

## 2. Curadoria de Fontes

Fontes selecionadas e carregadas no NotebookLM:

1. NIST. *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*. Disponível em: https://nvlpubs.nist.gov/nistpubs/ai/
2. NIST. *NIST AI RMF Playbook*. Disponível em: https://airc.nist.gov/AI_RMF_Knowledge_Base/Playbook
3. [Projeto01-DIO-PBI.pdf](https://unesdoc.unesco.org/in/documentViewer.xhtml?ark=%2Fark:%2F48223%2Fpf0000390241%2FPDF%2F390241por.pdf&file=%2Fin%2Frest%2FannotationSVC%2FDownloadWatermarkedAttachment%2Fattach_import_0880195e-d225-4872-bc95-e36b69d17343?_=390241por.pdf&id=p::usmarcdef_0000390241&locale=en&multi=true&v=2.1.196&utm_source=chatgpt.com)
4. Resources | Data Analysis for Social Science (MIT OpenCourseWare 14.310x)
5. STAT 508 | Applied Data Mining and Statistical Learning (Penn State)

---

## 3. Engenharia de Prompts e "Cicatrizes"

### Prompt 01 — Fundamentos da análise de dados

**Pergunta utilizada:**
> Utilizando exclusivamente as fontes disponibilizadas neste notebook, explique o que é análise de dados e descreva suas principais etapas. Para cada etapa, apresente sua finalidade, os principais conceitos envolvidos e indique quais fontes sustentam cada informação.

**Objetivo:** Compreender o conceito de análise de dados e identificar suas principais etapas, relacionando cada etapa às fontes utilizadas no NotebookLM.

**Resultado obtido:** O NotebookLM apresentou uma resposta estruturada em seis etapas (coleta e obtenção de dados; preparação e limpeza; análise exploratória; modelagem estatística e Machine Learning; avaliação e validação; implantação, operação, monitoramento e gestão), relacionando conceitos como amostragem, estatística descritiva, regressão, classificação, clustering, validação cruzada, overfitting, drift, explicabilidade e interpretabilidade.

**Pontos positivos:**
- Resposta organizada por etapas, com conceitos técnicos relevantes;
- Indicou as fontes utilizadas em cada seção;
- Relacionou análise de dados, estatística e Machine Learning.

**Problemas identificados:**
- Incluiu etapas (implantação e monitoramento de modelos de IA) mais próximas do ciclo de vida de sistemas de IA do que da análise de dados em si;
- Algumas fontes citadas não correspondiam claramente às 5 fontes selecionadas;
- Conceitos apresentados de forma muito técnica para um material introdutório;
- Misturou conceitos de estatística, Machine Learning e gestão de riscos de IA sem deixar clara a fronteira entre eles;
- Muita informação concentrada em uma única etapa.

**Aprendizado:** Um prompt detalhado gera resposta mais estruturada, mas pedir para "usar exclusivamente as fontes" não garante, por si só, que as relações conceituais estejam bem delimitadas. A próxima rodada precisava exigir separação clara entre análise de dados, estatística, Machine Learning, Inteligência Artificial e ciclo de vida de sistemas de IA.

**Próxima estratégia:** Pedir ao NotebookLM que utilize somente as fontes selecionadas, diferencie conceitos relacionados, sinalize explicitamente quando uma informação não estiver sustentada pelas fontes, evite extrapolações, cite as fontes específicas e use linguagem para iniciantes.

### Prompt 02 — Refinamento e diferenciação de conceitos

Aplicando os ajustes definidos após o Prompt 01, uma nova rodada de prompts no NotebookLM gerou um material mais avançado, com uma tabela de auditoria diferenciando explicitamente quais etapas pertencem à análise de dados clássica e quais são exclusivas do ciclo de vida de sistemas de IA. Os materiais disponíveis para consulta são o [miniguia em Markdown](./miniguia-ia-dados.md) e o [manual em PDF](./manual-ia-analise-dados.pdf).

---

## 4. Miniguia de Estudo (Entrega Final)

### 4.1 O que é análise de dados?
Estudo, planejamento e aplicação de métodos quantitativos para coletar, sintetizar, descrever e interpretar dados do mundo real, gerando conhecimento e subsidiando decisões.

### 4.2 Etapas da análise de dados
1. **Preparação de Dados** — obtenção, limpeza e transformação dos dados brutos.
2. **Análise Exploratória de Dados (EDA)** — visualização e estatísticas descritivas para entender distribuições e formular hipóteses.
3. **Análise e Modelagem** — ajuste de modelos supervisionados (regressão, classificação) ou não supervisionados (clustering).
4. **Avaliação e Validação** — testes em novos dados (validação cruzada), métricas como RMSE e matriz de confusão.
5. **Interpretação de Resultados** — tradução dos resultados matemáticos em conhecimento aplicável, distinguindo inferência de predição.

### 4.3 O que é Inteligência Artificial?
Segundo o NIST (AI RMF 1.0), um sistema de IA gera predições, recomendações ou decisões influenciando ambientes reais ou virtuais, com natureza **sócio-técnica** — seus riscos emergem da interação entre técnica, instituições e contexto social.

### 4.4 IA aplicada aos dados
- **Aprendizado Supervisionado:** classificação e regressão com dados rotulados (KNN, SVM, Árvores de Decisão, Redes Neurais).
- **Aprendizado Não Supervisionado:** identificação de padrões sem rótulos (Clustering, K-means).

### 4.5 IA Generativa
Subcampo que gera conteúdos novos (textos, código, imagens) a partir de prompts. LLMs funcionam de forma estatística/probabilística, prevendo a próxima palavra — por isso chamados de **"papagaios estocásticos"**.

### 4.6 Benefícios da IA na análise de dados
- Apoio na fase inicial de pesquisa (síntese bibliográfica);
- Redução de dimensionalidade (PCA);
- Estabilidade preditiva (Ensemble Learning);
- Identificação de variáveis mais relevantes (variable importance).

### 4.7 Limitações
- Alucinação (fabricação de fatos/referências);
- Opacidade ("caixas-pretas");
- Drift (desvios ao longo do tempo);
- Diferença entre desempenho em laboratório e em produção;
- Pegada ambiental do treinamento.

### 4.8 Vieses (NIST)
1. **Sistêmicos** — históricos e estruturais nos dados e na sociedade;
2. **Computacionais/Estatísticos** — amostragem não representativa;
3. **Cognitivos Humanos** — viés de automação (confiar cegamente na máquina).

### 4.9 Ética e privacidade
Uso de dados sem consentimento, violação de propriedade intelectual, e o risco de a interação humano-IA amplificar vieses cognitivos.

### 4.10 Papel do profissional de dados
Data Scientists, Data Engineers, Software Developers/System Integrators e times de TEVV (Teste, Avaliação, Verificação e Validação) — cada um com responsabilidades específicas no ciclo de governança.

### 4.11 Boas práticas (NIST AI RMF)
- **GOVERN** — cultura organizacional de transparência e responsabilidade;
- **MAP** — entender contexto legal, riscos e impactos sociais;
- **MEASURE** — testes de TEVV e monitoramento contínuo de drift;
- **MANAGE** — gestão de riscos com intervenção humana (human-in-the-loop).

### 4.12 Glossário
- **TEVV:** processos de Teste, Avaliação, Verificação e Validação ao longo do ciclo de vida da IA.
- **Data Wrangling:** manipulação, filtragem e reestruturação inicial dos dados.
- **Explicabilidade:** como o modelo funciona internamente.
- **Interpretabilidade:** o que o resultado do modelo significa na prática.
- **Concept Drift:** degradação do modelo por mudança nas relações entre dados e realidade.
- **Overfitting:** o modelo memoriza ruído dos dados de treino e perde capacidade de generalizar.

### 4.13 Prompts reutilizáveis para analistas de dados

**A. Revisão Bibliográfica e Triagem de Requisitos (papel de Explorador da UNESCO)**
```text
Atue como meu assistente de pesquisa científica e explorador bibliográfico de dados.
Preciso realizar o levantamento de conceitos fundamentais para a seguinte questão de pesquisa: "[INSERIR QUESTÃO DE PESQUISA]".

Para apoiar minha fase de preparação e desenho do estudo, realize as seguintes tarefas:
1. Resuma as principais teorias e abordagens clássicas associadas a esse problema.
2. Liste as variáveis e atributos mais comumente mensurados em estudos dessa natureza.
3. Identifique potenciais fontes públicas ou tipos de dados recomendados para este problema.

Restrições cruciais de segurança (UNESCO/NIST):
- Não invente referências bibliográficas. Se não tiver certeza de um artigo ou autor, declare explicitamente que não possui a confirmação documental.
- Mantenha um tom puramente neutro e identifique se os conceitos comuns que você listar herdam vieses históricos ou assimetrias de representação demográfica.
- Destaque quais limitações éticas de privacidade de dados eu devo considerar ao coletar estas informações.
```

**B. Apoio em Código e Transformação (Data Wrangling em R)**
```text
Atue como um especialista técnico em programação R e Data Wrangling.
Tenho uma base de dados estruturada chamada `df` com as seguintes variáveis originais: [LISTAR VARIÁVEIS].

Escreva um código em R limpo, documentado e defensivo para:
1. Subsetting: filtre as observações mantendo apenas os registros onde [NOME DA VARIÁVEL] atenda ao critério: [DESCREVER CRITÉRIO].
2. Seleção: selecione apenas as colunas essenciais: [LISTAR VARIÁVEIS ESSENCIAIS].
3. Criação de Atributos: crie uma nova variável `[NOME]` baseada na regra: [DESCREVER REGRA].

Garantias de qualidade:
- Trate valores nulos (NAs) antes das transformações.
- Comente cada linha do código.
- O script deve ser estático e pronto para execução.
```

**C. Explicabilidade e Interpretabilidade do Modelo (NIST AI RMF)**
```text
Atue como um especialista em auditoria e governança sócio-técnica de IA, seguindo o NIST AI RMF 1.0.
Acabo de ajustar um modelo preditivo de [TIPO DE MODELO] com as seguintes saídas:
- Variáveis mais importantes: [LISTAR VARIÁVEIS E PESOS]
- Métricas de erro: [INSERIR MÉTRICAS]

Estruture um relatório com:
1. EXPLICABILIDADE: como o algoritmo processa essas variáveis internamente.
2. INTERPRETABILIDADE: o que esse resultado significa na prática para um tomador de decisão não técnico.

Indique também:
- Que tipo de drift poderia comprometer esta interpretação no futuro?
- Há risco de viés de automação? Como mitigar?
```

**D. Desafio de Hipóteses (papel de Oponente Socrático da UNESCO)**
```text
Atue como meu oponente socrático acadêmico.
Formulei a seguinte hipótese: "[INSERIR SUA HIPÓTESE DE TRABALHO]"

Desafie criticamente esta hipótese para evitar viés de confirmação:
1. Questione premissas ocultas ou pressupostos não declarados.
2. Apresente duas explicações alternativas plausíveis.
3. Proponha testes estatísticos adicionais ou variáveis de controle para validar/refutar a hipótese.

Seu objetivo não é concordar comigo, mas expor fraquezas metodológicas de forma construtiva.
```

---

## 5. Material Complementar

Como aprofundamento, realizei uma rodada adicional de engenharia de prompts no NotebookLM, gerando um manual mais avançado com fronteiras mais nítidas entre análise de dados e ciclo de vida de IA, além de uma comparação entre os algoritmos KNN e SVM.

- 📄 [Manual de IA Aplicada à Análise de Dados — PDF](./manual-ia-analise-dados.pdf)
- 📚 [Miniguia de IA Aplicada à Análise de Dados — Markdown](./miniguia-ia-dados.md)

---

*Notebook original no NotebookLM (acesso pode ser restrito): [(https://notebook.google.com/notebook/455f904d-51d6-4a9c-8722-cfe47d97ab83)](https://notebook.google.com/notebook/455f904d-51d6-4a9c-8722-cfe47d97ab83)*
