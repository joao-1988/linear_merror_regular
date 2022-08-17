---
---

<h1><center><b>
MODELO LASSO PARA O PROBLEMA DE REGRESSÃO COM ERRO DE MEDIDA
</b></center></h1>

---
---

A regressão com a penalidade lasso é uma técnica bastante utilizada para realizar a redução de dimensão quando o número de covariáveis ​​é grande.

O artigo Measurement error in LASSO: Impact and likelihood bias correction [1] aborda o impacto do erro de medição na regressão linear com a penalidade do lasso, tanto analiticamente quanto em experimentos de simulação. Considera um método simples de correção para erro de medida no lasso. E mostra que no limite, o lasso corrigido produz uma seleção de covariáveis ​​consistente de sinal sob condições muito semelhantes ao lasso com medidas perfeitas, enquanto o lasso não corrigido requer condições muito mais rigorosas na estrutura de covariância dos dados.

Neste sentido, resolvi comparar os modelos Lasso com correção (abordagem utilizada em [1]), com Lasso sem correção e o Elastic Net para um problema de regressão com erro de medida nas covariadas. 

Os algorítmos destes modelos foram implementados em Python utilizando apenas o módulo Numpy para uma comparação mais justa de cada uma das abordagens. O detalhamento de cada algorítmo foi explicitado anteriormente a apresentação do código. Adicionalmente incluímos o modelo de regressão Linear.

## Referências Principais

[1] SØRENSEN, Øystein; FRIGESSI, Arnoldo; THORESEN, Magne. Measurement error in LASSO: Impact and likelihood bias correction. Statistica sinica, p. 809-829, 2015.

[2] FRIEDMAN, Jerome; HASTIE, Trevor; TIBSHIRANI, Rob. Regularization paths for generalized linear models via coordinate descent. Journal of statistical software, v. 33, n. 1, p. 1, 2010. Disponível em: <https://www.jstatsoft.org/article/view/v033i01/v33i01.pdf>

[3] LOH, Po-Ling; WAINWRIGHT, Martin J. High-dimensional regression with noisy and missing data: Provable guarantees with non-convexity. Advances in neural information processing systems, v. 24, 2011.

[4] Gradiente Descentende. Método do Gradiente Descendente. Disponível em: <https://ml-cheatsheet.readthedocs.io/en/latest/gradient_descent.html>
