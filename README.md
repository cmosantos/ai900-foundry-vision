# AI-900 – Labs de Visão com Microsoft Foundry 👁️‍🗨️☁️

Repositório com os labs que pratiquei para o exame **AI-900**, usando a experiência nova do **Microsoft Foundry (ai.azure.com)**:

- Análise de imagens (caption, tags, objetos)
- OCR / Content Understanding (invoice)
- Testes extras com minha própria imagem

Os recursos do Azure já foram apagados (para evitar custo), então aqui ficam apenas os **arquivos de dados** e a **descrição do que foi feito**.

---

## 📁 Estrutura deste repositório

- `data/images/`  
  Imagens usadas nos labs:
  - `store-camera-*.jpg` – imagens de exemplo do lab de Image Analysis (loja, câmeras etc.).
  - `claudio.jpg` – minha foto usada em testes de detecção de pessoa no Foundry (opcional).

- `data/docs/`  
  Documentos usados no lab:
  - `contoso-invoice-1.pdf` – invoice usada no lab de **Content Understanding / Invoice Data Extraction**.

---

## 🧪 Lab 1 – Image Analysis no Foundry

**Objetivo**

Explorar a análise de imagens no **Microsoft Foundry**, na seção:

> AI Services → Vision + Document → aba *Image*

Usando os recursos de:

- **Image captioning** – gerar uma legenda em texto descrevendo a imagem.
- **Dense captioning** – gerar várias legendas para diferentes regiões da imagem.
- **Common tag extraction** – gerar tags (palavras-chave) com score de confiança.
- **Common object detection** – detectar objetos/pessoas na imagem com bounding boxes.

**Arquivos**

As imagens usadas neste lab estão em:

- `data/images/store-camera-1.jpg`
- `data/images/store-camera-2.jpg`
- `data/images/store-camera-3.jpg`
- `data/images/store-camera-4.jpg`

---

## 🧾 Lab 2 – OCR e Content Understanding (Invoice)

**Objetivo**

Usar o **Content Understanding** no Foundry para extrair informações estruturadas de uma invoice (nota fiscal), como:

- Invoice ID  
- Invoice Date  
- Subtotal  
- Tax  
- Total  

**Como foi feito (resumo)**

- Criei um projeto de **Content Understanding** no Foundry.
- Usei o modelo de **Invoice Data Extraction**.
- Analisei o arquivo `contoso-invoice-1.pdf`, localizado em `data/docs/`.
- Vi na interface os campos detectados e também o resultado em **JSON**.

**Arquivo**

- `data/docs/contoso-invoice-1.pdf`

---

## 🙂 Lab 3 – Teste extra de visão com minha foto (Foundry)

**Objetivo**

Complementar o estudo de visão usando minha própria imagem no Foundry, em:

> AI Services → Vision + Document → aba *Image* → **Common object detection**

**O que foi feito**

- Subi uma imagem minha (`claudio.jpg`) no Foundry.
- O modelo detectou o objeto **`person`** na imagem.
- A interface mostrou:
  - Um **bounding box** (quadrado) em volta do meu rosto/corpo.
  - Um **score de confiança**, por exemplo: `person (86.80%)`.
  - Um controle de **Threshold value** para ajustar o score mínimo exibido.

**Arquivo (opcional)**

- `data/images/claudio.jpg` – só será incluído se eu quiser expor a foto no GitHub.

---

## ✅ O que esses labs cobrem para o AI-900

- Conceitos de **visão computacional** no Azure:
  - legendas de imagem,
  - tags,
  - detecção de objetos/pessoas.
- Conceitos de **OCR** e **extração de dados estruturados** com Content Understanding.
- Experiência prática com o **Microsoft Foundry**, a plataforma nova da Microsoft para trabalhar com Azure AI.

---
