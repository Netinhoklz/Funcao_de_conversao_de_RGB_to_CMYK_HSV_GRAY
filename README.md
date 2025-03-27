# Visão Computacional e Processamento de Imagens

Trabalho realizado para a disciplina de Visão Computacional e Processamento de Imagens no Laboratório de Ciência de Dados e Inteligência Artificial (LCDIA) da Universidade de Fortaleza.

- **Aluno:** José Freitas Alves Neto
- **Professor:** Rilder de Sousa Pires

## Objetivo

O objetivo principal deste trabalho é implementar funções para a conversão entre diferentes modelos de cores de imagens, utilizando Python e conceitos de processamento de imagens.

## Conversões Implementadas

O notebook (`.ipynb`) contém a implementação das seguintes funções de conversão de modelos de cores:

1.  **RGB para Escala de Cinza (Grayscale):** Converte uma imagem colorida (RGB) para sua representação em tons de cinza utilizando a fórmula de luminância:
    `Grayscale = 0.299*R + 0.587*G + 0.114*B`
2.  **RGB para CMYK:** Converte uma imagem RGB para o modelo de cores CMYK (Ciano, Magenta, Amarelo, Preto).
3.  **RGB para HSV:** Converte uma imagem RGB para o modelo de cores HSV (Matiz, Saturação, Valor).
    *Nota: A implementação segue o padrão matemático onde H ∈ [0, 360), S ∈ [0, 1], e V ∈ [0, 1].*

## Validação

As funções implementadas foram validadas:
- A conversão RGB para Grayscale foi comparada com o resultado da função `cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)`.
- A conversão RGB para CMYK foi validada revertendo a transformação CMYK para RGB e comparando visualmente com a imagem original.
- A conversão RGB para HSV foi comparada com o resultado da função `colorsys.rgb_to_hsv` para cores de teste.

## Tecnologias Utilizadas

- Python 3
- NumPy
- Matplotlib
- OpenCV (`cv2`)
- colorsys
- Google Colab (ou ambiente Jupyter com `gdown` para baixar as imagens de exemplo)

## Como Usar

1.  Clone o repositório.
2.  Abra o arquivo `.ipynb` em um ambiente compatível (Jupyter Notebook, Google Colab, VS Code, etc.).
3.  Execute as células sequencialmente. A primeira célula de código fará o download das imagens de exemplo necessárias usando `gdown`.
4.  Observe as transformações e validações nas saídas das células.
