# Sistema de Recomendação por Imagens

Este repositório contém o código para um sistema de recomendação baseado em similaridade de imagens, utilizando o dataset "Ecommerce Product Images - 18k" do Kaggle.

## Descrição

O sistema usa o modelo CLIP para extrair embeddings de imagens de produtos (cerca de 18.000, divididas em 9 categorias como BEAUTY_HEALTH e ELECTRONICS). Os embeddings são indexados com FAISS para buscas rápidas, e o resultado inclui recomendações visuais testadas com imagens do dataset ou uploads.

## Estrutura

Pré-processamento: Download via kagglehub, filtragem de um subconjunto de 2.250 imagens.
Extração: Geração de embeddings com CLIP (512 dimensões).
Indexação: Uso de FAISS para eficiência.
Teste: Exibição de imagens de entrada e recomendações com matplotlib.
