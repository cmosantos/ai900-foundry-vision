# AI-900 – Labs de Visão com Microsoft Foundry 👁️‍🗨️☁️

Repositório com os labs que pratiquei para o exame **AI-900**, usando a experiência nova do **Microsoft Foundry (ai.azure.com)**:

- Análise de imagens (caption, tags, objetos)
- OCR / Content Understanding (invoice)
- Testes extras com minha própria imagem

Os recursos do Azure já foram apagados (para evitar custo). Aqui ficam apenas os arquivos de dados e a descrição do que foi feito.

---

## 📁 Arquivos deste repositório

- `store-camera-1.jpg`  
- `store-camera-2.jpg`  
- `store-camera-3.jpg`  
- `store-camera-4.jpg`  
  > Imagens de exemplo usadas nos labs de **Image Analysis** (Vision + Document – aba *Image*).

- `claudio.jpg` *(opcional)*  
  > Minha foto usada em **Common object detection** no Foundry para testar detecção de pessoa.

- `contoso-invoice-1.pdf` *(vou subir depois)*  
  > Invoice usada no lab de **Content Understanding / Invoice Data Extraction**.

---

## 🧪 Lab 1 – Image Analysis no Foundry

**Objetivo**

Explorar a análise de imagens no **Microsoft Foundry**, em:

> AI Services → Vision + Document → aba *Image*

Usando:

- **Image captioning** – gerar uma legenda em texto descrevendo a imagem.  
- **Dense captioning** – gerar várias legendas para diferentes regiões.  
- **Common tag extraction** – gerar tags com score de confiança.  
- **Common object detection** – detectar objetos/pessoas com bounding boxes.

**Imagens usadas**

- `store-camera-1.jpg`
- `store-camera-2.jpg`
- `store-camera-3.jpg`
- `store-camera-4.jpg`

---

## 🧾 Lab 2 – OCR / Content Understanding (Invoice)

**Objetivo**

Usar **Content Understanding** no Foundry para extrair dados estruturados de uma invoice:

- Invoice ID  
- Invoice Date  
- Subtotal  
- Tax  
- Total  

**Como foi feito (resumo)**

- Criei um projeto de **Content Understanding** no Foundry.  
- Usei o modelo de **Invoice Data Extraction**.  
- Analisei o arquivo `contoso-invoice-1.pdf`.  
- Conferi os campos detectados na interface e o resultado em **JSON**.

---

## 🙂 Lab 3 – Teste extra de visão com minha foto

**Objetivo**

Complementar o estudo de visão usando minha própria imagem em:

> AI Services → Vision + Document → aba *Image* → **Common object detection**

**O que aconteceu**

- Subi a imagem `claudio.jpg` no Foundry.  
- O modelo detectou o objeto **`person`**.  
- A interface mostrou:
  - um **bounding box** em volta da pessoa;  
  - um **score de confiança**, ex.: `person (86.80%)`;  
  - um controle de **Threshold value** para ajustar o score mínimo.

---

## ✅ O que esses labs cobrem para o AI-900

- Conceitos de **visão computacional** no Azure:
  - legendas de imagem,
  - tags,
  - detecção de objetos/pessoas.
- Conceitos de **OCR** e extração de dados estruturados com Content Understanding.
- Experiência prática com o **Microsoft Foundry**, a plataforma nova de Azure AI.

---
