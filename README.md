# Projeto 10

Implementação e Análise de Classificação com Redes Convolucionais e o dataset CUFS - Unidade 10 - Trilha Ciência de Dados - RESTIC 36.
Este projeto implementa um Classificador de Gênero utilizando uma Rede Neural Convolucional (CNN) em linguagem Python. O modelo é capaz de classificar imagens de rostos em duas categorias: feminino e masculino.

## Requisitos

- Python 3.8+
- TensorFlow 2.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- PIL (Pillow)
- scikit-learn

Para instalar as dependências:
```bash
pip install -r requirements.txt
```

## Estrutura do Projeto

- `Projeto10.ipynb`: Notebook principal com o algoritmo desenvolvido
- `Relatorio_Tecnico_CNN.pdf`: Relatório técnico completo sobre o projeto
- `requirements.txt`: Lista de dependências do projeto

## Como Usar

1. **Preparação do Ambiente**
   - Clone o repositório
   - Instale as dependências

2. **Executando o Notebook**
   - Abra o `Projeto10.ipynb` no Jupyter Notebook
   - Execute as células em ordem
   - O notebook está dividido em seções claras para fácil navegação

3. **Estrutura do Notebook**
   - Importação de bibliotecas
   - Carregamento e pré-processamento dos dados
   - Definição e treinamento do modelo
   - Avaliação e visualização dos resultados
   - Função para predições em novas imagens
     
## Dataset

- O modelo foi treinado com o dataset CUHK Face Sketch
- As imagens são redimensionadas para 250x200 pixels durante o processamento
- Data augmentation é aplicado na classe 'feminino' para melhorar a generalização

## Arquitetura do Modelo

A CNN implementada possui a seguinte arquitetura:
- Input: Imagens RGB (200x250 pixels)
- 3 camadas convolucionais com MaxPooling
- Camadas densas com dropout
- Saída: Classificação binária (Feminino/Masculino)

## Avaliação do Modelo

O modelo é avaliado usando:
- Acurácia de treino e validação
- Matriz de confusão
- Curva ROC e AUC
- F1-Score
- Recall e Precision

## Resultados

O modelo é capaz de:
- Processar imagens de diferentes tamanhos
- Classificar gênero com boa acurácia
- Fornecer nível de confiança para cada predição
- Lidar com diferentes formatos de imagem
