# Calculo-de-metricas
Cálculo de métricas de uma matriz de confusão


# Avaliação de Classificadores com Métricas Estatísticas

Este script em Python calcula métricas clássicas de avaliação de modelos de classificação binária com base nos valores da matriz de confusão.

## Métricas Calculadas

As métricas implementadas no código são:

### Sensibilidade (Recall)

Indica a proporção de verdadeiros positivos identificados corretamente pelo modelo.

Fórmula:

Recall = VP / (VP + FN)



### Especificidade

Indica a proporção de verdadeiros negativos corretamente classificados.

Fórmula:


Especificidade = VN / (VN + FN)



### Acurácia

Proporção de todas as previsões corretas (positivas e negativas) em relação ao total de amostras.

Fórmula:


Acurácia = (VP + VN) / N



### Precisão (Precision)

Indica a proporção de previsões positivas que são realmente positivas.

Fórmula:


Precisão = VP / (VP + FP)



### F1-Score

Média harmônica entre precisão e sensibilidade. Útil especialmente em cenários com classes desbalanceadas.

Fórmula:


F1-Score = 2 \* (Precisão \* Recall) / (Precisão + Recall)



## Código

recall = Vp / (Vp + Fn)
espec = Vn / (Fn + Vn)
accuracy = (Vp + Vn) / N
precision = Vp / (Vp + Fp)
f_score = 2 * (precision * recall) / (precision + recall)

print(f"Sensibilidade: {recall*100:.2f}%")

print(f"Especificidade: {espec*100:.2f}%")

print(f"Acuracia: {accuracy*100:.2f}%")

print(f"Precisão: {precision*100:.2f}%")

print(f"f_score: {f_score*100:.2f}%")


## Exemplo de Uso

Antes de executar o código, defina os valores da matriz de confusão, como no exemplo abaixo:

python
Vp = 950   # Verdadeiros Positivos
Vn = 9040  # Verdadeiros Negativos
Fp = 2     # Falsos Positivos
Fn = 8     # Falsos Negativos
N = 10000  # Total de amostras


Execute o script para obter as métricas em formato percentual com duas casas decimais.

## Requisitos

* Python 3.x

Este script é útil para análise de desempenho de classificadores binários, como em problemas de detecção de doenças, filtros de spam, reconhecimento de padrões, entre outros.

