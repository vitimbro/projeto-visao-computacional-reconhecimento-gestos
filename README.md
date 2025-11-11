# Projeto: Reconhecimento de Gestos Manuais com MediaPipe

Este projeto é uma aplicação de visão computacional desenvolvida com o objetivo de realizar o reconhecimento de gestos com as mãos em tempo real. Utilizando a biblioteca MediaPipe do Google, o sistema identifica a posição da mão e mapeia seus 21 pontos de referência (landmarks) para interpretar movimentos e classificá-los como gestos específicos.

Este repositório contém o notebook Jupyter (`.ipynb`) com todo o processo de desenvolvimento, análise e implementação do sistema.

## Tabela de Conteúdos

  * [Visão Geral do Projeto](https://www.google.com/search?q=%23-vis%C3%A3o-geral-do-projeto)
  * [Principais Funcionalidades](https://www.google.com/search?q=%23-principais-funcionalidades)
  * [Tecnologias Utilizadas](https://www.google.com/search?q=%23-tecnologias-utilizadas)
  * [Como Acessar e Executar](https://www.google.com/search?q=%23-como-acessar-e-executar)
  * [Metodologia e Desenvolvimento](https://www.google.com/search?q=%23-metodologia-e-desenvolvimento)
  * [Testes Realizados](https://www.google.com/search?q=%23-testes-realizados)

## Visão Geral do Projeto

O objetivo central é criar um sistema robusto para a interpretação de gestos manuais capturados por uma webcam. A aplicação analisa o frame de vídeo, detecta a presença de mãos e extrai uma malha de 21 pontos-chave. Com base na posição relativa desses pontos, o sistema é capaz de classificar diferentes gestos.

## Principais Funcionalidades

  * **Detecção de Mãos em Tempo Real:** Identifica e rastreia mãos no feed de vídeo.
  * **Mapeamento de Landmarks:** Extrai 21 pontos de referência (landmarks) da mão, permitindo uma análise detalhada da sua pose.
  * **Classificação de Gestos:** Interpreta a posição dos landmarks para identificar gestos pré-definidos (ex: "punho fechado", "mão aberta", "sinal de positivo").

## Tecnologias Utilizadas

  * **Python 3**
  * **Google Colab**
  * **MediaPipe:** Biblioteca principal para detecção de mãos e landmarks.
  * **OpenCV:** Utilizado para captura e processamento do feed de vídeo (webcam).

## 🚀 Como Acessar e Executar

### Acesso Rápido (Recomendado): Google Colab

A forma mais simples de interagir com o projeto é abri-lo diretamente no Google Colab, que gerencia todas as dependências automaticamente no navegador.

1.  Acesse o arquivo do notebook neste repositório:
    [**`Projeto_de_Visão_Computacional_Reconhecimento_de_Gestos_Manuais.ipynb`**](https://www.google.com/search?q=Projeto_de_Vis%C3%A3o_Computacional_Reconhecimento_de_Gestos_Manuais.ipynb)
2.  No topo da visualização do arquivo, clique no ícone **"Open in Colab"**.
3.  Uma nova aba será aberta com o notebook no ambiente do Colab.
4.  Execute as células de código sequencialmente (usando "Shift + Enter" ou o botão "Play").

## 🛠️ Metodologia e Desenvolvimento

O desenvolvimento seguiu uma abordagem iterativa. Inicialmente, foram testadas técnicas mais tradicionais de visão computacional com OpenCV, como a detecção baseada em cor (thresholding de HSL/HSV) e a análise de contornos.

Embora funcionais em ambientes controlados, essas abordagens mostraram-se sensíveis a variações de iluminação e complexidade do fundo. Diante disso, optou-se pela migração para a biblioteca **MediaPipe**, que oferece modelos pré-treinados de alta performance, resultando em uma detecção significativamente mais precisa e eficiente.

## 🧪 Testes Realizados

Para validar a robustez do sistema final, foram realizados testes em múltiplos cenários, variando:

  * **Condições de Luz:** (Ambientes claros, escuros e com luz artificial).
  * **Ângulo da Câmera:** (Frontal, lateral, superior).
  * **Ambiente de Fundo:** (Fundos simples e fundos complexos/movimentados).
