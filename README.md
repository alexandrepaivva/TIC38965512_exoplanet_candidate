[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/alexandrepaivva/TIC38965512_Colab_Exoplanet/blob/main/analise_TIC38965512.ipynb)

# Analise inicial do candidato a exoplaneta TIC 38965512 com dados do TESS (Google Colab)

Este repositório contém um notebook Python desenvolvido para ser executado inteiramente no **Google Colab**. Ainda é possível executá-lo em outro ambiente que tenha linguagem de programação Python.

## Sobre o Projeto

O notebook baixa os dados do satélite TESS (setor 96), aplica o método **Box Least Squares (BLS)** para estimar o período orbital do candidato, calcula o raio planetário e o semi-eixo maior, e propaga as incertezas.

## Como executar

1. Clique no botão **"Open In Colab"** acima.
2. Execute as células em ordem (Shift + Enter).
3. Os gráficos e resultados serão gerados diretamente no ambiente do Colab.

## Dependências

Todas as bibliotecas são instaladas automaticamente pela primeira célula do notebook.

## Resultados esperados

Ao final da execução, serão exibidos no terminal do Colab:
- Período orbital (P) em dias.
- Raio do planeta em Raios de Júpiter e Raios da Terra.
- Semi-eixo maior (a) em Unidades Astronômicas (UA).
- Incertezas propagadas para o raio e semi-eixo maior.

Além disso, três gráficos serão salvos e exibidos:
- Curva de Luz Tratada
- Periodograma BLS
- Curva de Luz Dobrada (Folded)

## Análise de outras estrelas
Para reproduzir a análise em outras estrelas, basta substituir onde está indicado no código.
- Rotina 2: substituir o número do TIC_ID em "TIC_ID = "38965512"", retirar "38965512" e colocar dentro das aspas o número do TIC_ID da estrela que se deseja analisar.
- Rotina 3: substituir o número "96" que corresponde ao setor analisado, por um dos setores que deseja ser analisado da estrela, em "sector=96".
- Rotina 5: retirar o delimitador do eixo X - "plt.xlim(-0.4, 0.4)".
- Rotina 6: substituir os valores de raio e massa da estrela pelo valores de raio e massa da estrela que se deseja analisar, em "R_star = 1.0785 * R_sun" e "M_star = 1.01 * M_sun".
- Rotina 7: substituir as incertezas do raio e da massa estelar pelas incertezas da estrela que se deseja analisar, em "R_star_err_plus  = 0 * R_sun" erro para cima, "R_star_err_minus = 0 * R_sun erro para baixo" e "M_star_err_plus  = 0 * M_sun" erro para cima, "M_star_err_minus = 0 * M_sun erro para baixo".

---

**Contexto:** Trabalho acadêmico de análise de dados astronômicos.
