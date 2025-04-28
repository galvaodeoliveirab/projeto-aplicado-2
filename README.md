<img src="https://capsule-render.vercel.app/api?type=waving&color=FF6666&height=120&section=header" width="100%" align="center">

<img src="http://meusite.mackenzie.br/rogerio/mackenzie_logo/UPM.2_horizontal_vermelho.jpg" width="100%" align="center">
<br><br><br>

# **Projeto de Classificação de Publicações Judiciais 📄⚖️**  
Automação na Organização de Documentos Jurídicos  
Universidade Presbiteriana Mackenzie 🏫  
Faculdade de Computação e Informática 💻  

## **Autores**  
- **Bruno Galvão de Oliveira Lima** – TIA: 10441285  
- **Vitória Ferreira Corrêa** – TIA: 10441482  
- **Lucas Santos Borba de Araujo** – TIA: 10176256  
- **Anna Teresa Soares Sacchi** – TIA: 10441273  

## **Docente**  
- **Prof. Felipe Albino dos Santos**

**São Paulo – 2025**

---

## **Resumo**

Este projeto propõe a classificação automatizada de textos jurídicos obtidos via API do Processo Judicial Eletrônico (PJe), segmentando as publicações em categorias como Citação, Intimação, Edital e Lista de Distribuição.  

A empresa fictícia **Data for You SA** representa uma solução inovadora para a padronização e otimização do acesso a documentos jurídicos.  

O trabalho utiliza técnicas de Processamento de Linguagem Natural (PLN), vetorização TF-IDF e algoritmos supervisionados como Random Forest. Os dados são armazenados em um banco de dados PostgreSQL.

---

## **Sumário**

1. [Introdução](#introdução)  
2. [Definição da Empresa](#definição-da-empresa)  
   - 2.1 Identificação e Propósito  
   - 2.2 Segmento de Atuação e Market Share  
   - 2.3 Problema de Pesquisa  
   - 2.4 Fonte e Aquisição dos Dados  
3. [Apresentação dos Dados (Metadados)](#apresentação-dos-dados-metadados)  
   - 3.1 Fonte e Estrutura  
   - 3.2 Análise Exploratória  
   - 3.3 Linguagem de Programação e Bibliotecas  
   - 3.4 Tratamento de Dados  
   - 3.5 Bases Teóricas dos Métodos  
   - 3.6 Avaliação de Acurácia  
4. [Objetivos e Metas](#objetivos-e-metas)  
5. [Storytelling](#storytelling)  
6. [Produto Final e Modelo de Negócio](#produto-final-e-modelo-de-negócio)  
7. [Conclusão](#conclusão)  
8. [Repositório](#repositório)

---

## **1. Introdução**

O projeto surgiu para solucionar a dificuldade de triagem de publicações judiciais no meio jurídico. Utilizando PLN e Machine Learning, construímos um modelo preditivo capaz de automatizar a categorização desses documentos.

---

## **2. Definição da Empresa**

### 2.1 Identificação e Propósito  
Empresa fictícia: **Data for You SA**  
Missão: Democratizar o acesso a dados jurídicos por meio de soluções open source.

### 2.2 Segmento de Atuação e Market Share  
Colaboração com CNJ, tribunais estaduais, federais e escritórios de advocacia.

### 2.3 Problema de Pesquisa  
A falta de padronização nas publicações judiciais dificulta sua análise e gestão.

### 2.4 Fonte e Aquisição dos Dados  
API do Processo Judicial Eletrônico (PJe), abrangendo publicações de 2013 a 2025.

---

## **3. Apresentação dos Dados (Metadados)**

### 3.1 Fonte e Estrutura  
A base de dados é composta por três colunas: `id`, `tipoComunicacao`, `texto`.

### 3.2 Análise Exploratória  
- 10.000 registros
- 5 categorias principais de publicações
- Tamanho médio dos textos: ~2.000 caracteres

### 3.3 Linguagem de Programação e Bibliotecas  
Utilizamos **Python** com as seguintes bibliotecas:
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn
- TfidfVectorizer

### 3.4 Tratamento de Dados  
- Normalização textual  
- Tokenização  
- Remoção de stopwords  
- Vetorização TF-IDF  
- Split treino/teste 80/20

### 3.5 Bases Teóricas dos Métodos  
Modelos testados:
- Random Forest
- Regressão Logística
- Naive Bayes
- Redes Neurais

### 3.6 Avaliação de Acurácia  
- **Acurácia final:** 91,67%  
- **Precisão média:** 91,78%  
- **Recall médio:** 91,67%  
- **F1-Score médio:** 91,57%

---

## **4. Objetivos e Metas**

- Coletar e tratar dados do PJe  
- Definir categorias jurídicas  
- Desenvolver um modelo supervisionado  
- Armazenar previsões em banco de dados  
- Avaliar o desempenho com métricas sólidas  
- Criar um fluxo automatizado para novas publicações

---

## **5. Storytelling**

Identificamos o problema de desorganização das publicações judiciais e propusemos uma solução baseada em PLN e Machine Learning. Após coletar, limpar e preparar os dados, treinamos um modelo Random Forest com ótimos resultados, reduzindo significativamente o tempo de categorização manual e otimizando o acesso à informação para profissionais do direito.

---

## **6. Produto Final e Modelo de Negócio**

### Produto Final  
- Sistema Automatizado de Classificação de Publicações Judiciais
- Armazenamento PostgreSQL
- Interface para consulta e análise

### Modelo de Negócio  
- Público-alvo: Escritórios jurídicos e órgãos públicos  
- Entrega: SaaS ou API  
- Benefícios: Redução de tempo e aumento de eficiência jurídica

---

## **7. Conclusão**

O projeto validou o uso de Machine Learning para classificação de documentos jurídicos. Com resultados superiores a 91% de acurácia, a solução mostrou-se viável tanto técnica quanto comercialmente.

---

## **8. Repositório**

🔗 GitHub: [https://github.com/galvaodeoliveirab/projeto-aplicado-2](https://github.com/galvaodeoliveirab/projeto-aplicado-2)

---

<img src="https://capsule-render.vercel.app/api?type=waving&color=FF6666&height=120&section=footer" width="100%" align="center">
