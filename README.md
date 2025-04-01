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

Este projeto propõe a classificação automatizada de textos jurídicos obtidos via API do Processo Judicial Eletrônico (PJe), segmentando as publicações em categorias como Citação, Intimação, Despacho e Decisão. A empresa fictícia **Data for You SA** representa uma solução inovadora para organização e acesso a documentos jurídicos.

O trabalho utiliza técnicas de Processamento de Linguagem Natural (PLN), vetorização TF-IDF e algoritmos supervisionados como Random Forest e Regressão Logística. Os dados são armazenados em um banco de dados PostgreSQL.

---

## **Sumário**

1. [Introdução](#introdução)  
2. [Definição da Empresa](#definição-da-empresa)  
   - 2.1 Identificação e Propósito  
   - 2.2 Segmento de Atuação e Market Share  
   - 2.3 Problema de Pesquisa  
   - 2.4 Fonte e Aquisição dos Dados  
3. [Apresentação dos Dados (Metadados)](#apresentação-dos-dados)  
   - 3.1 Fonte e Estrutura  
   - 3.2 Análise Exploratória  
   - 3.3 Linguagem de Programação  
   - 3.3.1 Bibliotecas Utilizadas  
   - 3.4 Tratamento de Dados  
   - 3.5 Bases Teóricas dos Métodos  
   - 3.6 Avaliação e Acurácia  
4. [Objetivos e Metas](#objetivos-e-metas)  
   - 4.1 Objetivo Geral  
   - 4.2 Objetivos Específicos  
5. [Cronograma](#cronograma)  
6. [Repositório](#repositório)

---

## **1. Introdução**

Com base nos desafios enfrentados por advogados e servidores, este projeto visa desenvolver um modelo preditivo para classificar publicações do PJe com apoio de PLN e aprendizado supervisionado. A solução proposta visa automatizar a triagem e reduzir o tempo de análise.

---

## **2. Definição da Empresa**

### 2.1 Identificação e Propósito  
Empresa fictícia: **Data for You SA**  
Missão: Democratizar o acesso a dados jurídicos.  
Visão: Criar soluções open source para automação jurídica.

### 2.2 Segmento de Atuação e Market Share  
Foco em análise de dados jurídicos em parceria com CNJ, tribunais e escritórios de advocacia.

### 2.3 Problema de Pesquisa  
A ausência de padronização nas publicações dificulta sua análise e organização.

### 2.4 Fonte e Aquisição dos Dados  
API do PJe, com dados coletados de 2013 até 2025.

---

## **3. Apresentação dos Dados**

### 3.1 Fonte e Estrutura  
A base contém três colunas principais: `id`, `tipoComunicacao`, `texto`.

### 3.2 Análise Exploratória  
Foram analisados:
- Frequência de cada tipo de publicação  
- Comprimento dos textos  
- Distribuição de classes

### 3.3 Linguagem de Programação  
Foi utilizada a linguagem **Python** por sua robustez em PLN e modelagem preditiva.

#### 3.3.1 Bibliotecas Utilizadas  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Scikit-learn  
- TfidfVectorizer

### 3.4 Tratamento de Dados  
- Conversão de tipos  
- Remoção de nulos e caracteres especiais  
- Tokenização  
- Stopwords personalizadas  
- Vetorização TF-IDF  
- Divisão treino/teste

### 3.5 Bases Teóricas dos Métodos  
Modelos aplicados:  
- Regressão Logística  
- Random Forest  
- Naive Bayes  
- Redes Neurais

### 3.6 Avaliação e Acurácia

#### 3.6.1 Divisão de Dados  
80% treino / 20% teste com `random_state=42`.

#### 3.6.2 Vetorização  
TF-IDF com stopwords definidas manualmente.

#### 3.6.3 Modelo  
Utilizado: **Random Forest** (bom desempenho em dados textuais).

#### 3.6.4 Métricas de Avaliação

- **Precisão (Precision):**  
  \[
  \text{Precisão} = \frac{TP}{TP + FP}
  \]

- **Revocação (Recall):**  
  \[
  \text{Recall} = \frac{TP}{TP + FN}
  \]

- **F1-Score:**  
  \[
  F_1 = 2 \cdot \frac{\text{Precisão} \cdot \text{Recall}}{\text{Precisão} + \text{Recall}}
  \]

- **Acurácia:**  
  \[
  \text{Acurácia} = \frac{TP + TN}{TP + TN + FP + FN}
  \]

#### 3.6.5 Aprimoramento Futuro  
Sugere-se aplicar validação cruzada com `cross_val_score` para obter desempenho médio mais confiável.

---

## **4. Objetivos e Metas**

### 4.1 Objetivo Geral  
Automatizar a categorização de publicações judiciais via PLN e Machine Learning.

### 4.2 Objetivos Específicos  
- Coleta via API do PJe  
- Pré-processamento textual  
- Aplicação de modelos supervisionados  
- Armazenamento em PostgreSQL  
- Avaliação com métricas robustas  
- Implementação de pipeline contínuo  
- Criação de interface para consulta

---

## **5. Cronograma**

Veja o cronograma detalhado com marcos e entregas no [relatório completo](https://github.com/galvaodeoliveirab/projeto-aplicado-2).

---

## **6. Repositório**

🔗 GitHub: [https://github.com/galvaodeoliveirab/projeto-aplicado-2](https://github.com/galvaodeoliveirab/projeto-aplicado-2)

---

<img src="https://capsule-render.vercel.app/api?type=waving&color=FF6666&height=120&section=footer" width="100%" align="center">
