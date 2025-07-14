# Classificação de Raças de Cachorros com CNN e VGG16

Este projeto utiliza redes neurais convolucionais (CNNs), incluindo uma arquitetura personalizada e a pré-treinada VGG16, para classificar imagens de cães em quatro raças distintas:

- **Spaniel**
- **Retriever**
- **Hound**
- **Terrier**

## 📁 Estrutura do Projeto

- `cnn_dogs_api.ipynb`: Notebook principal contendo todas as etapas do projeto, desde o pré-processamento até a avaliação dos modelos.

## 📊 Objetivo

Desenvolver e comparar o desempenho de duas abordagens:

1. **CNN personalizada** criada do zero com Keras.
2. **VGG16**, uma rede convolucional profunda pré-treinada, adaptada via *transfer learning*.

## 🐶 Conjunto de Dados

As imagens são divididas em quatro pastas, correspondentes a cada raça. Cada imagem foi redimensionada e normalizada para ser utilizada nos modelos.

**Observações:**
- O dataset está organizado em diretórios, seguindo o padrão esperado pelo `ImageDataGenerator`.
- As imagens são separadas em conjuntos de treino e validação.

## ⚙️ Tecnologias e Bibliotecas

- Python 3
- TensorFlow / Keras
- NumPy
- Matplotlib
- Google Colab (para execução)

## 🧠 Modelos Utilizados

### CNN Personalizada

- Convoluções com ReLU e max-pooling
- Camadas fully connected
- Dropout para regularização
- Otimização com Adam
- Treinamento por várias épocas com `EarlyStopping`

### VGG16

- Modelo pré-treinado no ImageNet
- Camadas convolucionais congeladas
- Adição de camadas densas no topo
- *Fine-tuning* opcional para melhorar desempenho
- Otimização com Adam

## 📈 Avaliação

- Acurácia por época nos conjuntos de treino e validação
- Visualização da matriz de confusão
- Relatório de classificação (precision, recall e F1-score)

## 📦 Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repo.git
