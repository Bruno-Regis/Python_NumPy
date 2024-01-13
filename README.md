# Curso de Numpy - Alura
## Tecnologias
<div> <img src="https://img.shields.io/badge/Python-%233776AB?style=for-the-badge&logo=python&logoColor=white"
<div> <img src="https://img.shields.io/badge/NumPy-%23F2F2F2?style=for-the-badge&logo=Numpy&logoColor=blue"
<div> <img src="https://img.shields.io/badge/Jupyter-%23CCCCCC?style=for-the-badge&logo=Jupyter&logoColor=orange"
<div> <img src="https://img.shields.io/badge/LateX-%236f6961?style=for-the-badge&logo=LateX&logoColor=%2357b3ac"
<div> <img src="https://img.shields.io/badge/Git-%23F2F2F2?style=for-the-badge&logo=Git&logoColor=orange"

## 1. Introdução
<div style="text-align: justify">
O curso de NumPy da Alura foi palco de estudo para efetivação do presente projeto.<br>
NumPy é uma biblioteca popular em Python para computação numérica. Ela fornece suporte para arrays multidimensionais e funções matemáticas para trabalhar com esses arrays. NumPy é uma base essencial para muitas outras bibliotecas científicas e de dados em Python devido à sua eficiência e facilidade de uso. <br>
Para efetivar o estudo, foram utilizados dois datasets do Kaggle, um chamado apples_ts.csv que fornece dados de preços de maçâs para cidades da Rússia, e outro dataset que foi utilizado no desafio do curso chamado citrus.csv que fornece informações de duas frutas, contendo dados como peso, diâmetro e espectrometria que no caso não foi estudada neste trabalho.
</div>

<div style="text-align: justify">
    
## 2. Objetivos
* Desvendar diversas funções da íncrivel biblioteca NumPy;
* Visualizar dados fornecidos pela Alura, disponíveis no Kaggle;
* Efetuar método estatístico para obter uma reta ajustada que represente os dados do dataset;
* Gerar milhares de dados aleatórios com a biblioteca NumPy a fim de encontrar os melhores resultados.

## 3. Métodos
### 3.1 Imports
As bibliotecas importadas foram:

* Numpy.
* Matplotlib.
### 3.2 Carregamento e processamento dos dados
Primeiramente, foram carregados os dados dos arquivos csv por meio da função loadtxt da numpy para efetuar as primeiras análises e tratamento dos dados.

    
### 3.3 Visualização dos dados
<div style="text-align: justify">
Os dados foram plotados utilizando a biblioteca matplotlib e as primeiras impressões do comportamento foram feitas. 
Criei um loop inteligente com for capaz de detectar e me indicar valores do tipo NaN (not a number), embora o curso não tenha aprofundado tanto nesta questão de tratamento e limpeza de dados, por ser mais focado na utilização da NumPy, foi possível de tratar os valores Nans e inserir a média dos valores vizinhos no seu index.
</div>

## 4. Regressão linear
<div style="text-align: justify">
A regressão linear é um método estatístico utilizado para modelar a relação entre uma variável dependente entre uma ou mais variáveis independentes. Isto é, o método tem como objetivo encontrar uma reta ajustada que melhor se encaixe aos dados observados. A equação da reta é representada por: <br> 
$$ Y = aX + b$$
Onde:<br>
$Y$ = Variável dependente;<br>
$X$ = Variável independente;<br>
$a$ = Inclinação da reta;<br>
$b$ = Interceptação no eixo Y;<br>
    
### 4.1 Cálculo do Coeficiente Angular da Reta (a): <br>
$$ \hat{a} = \frac{N\cdot\sum_{}^{}\left( X_{i}\cdot Y_{i} \right) - \sum_{_{}}^{}\left( X_{i} \right) \cdot \sum_{_{}}^{}\left( Y_{i} \right)} {N\cdot \sum_{_{}}^{}\left( X^{2}_{i} \right)-\left( \sum_{_{}}^{}\left( X_{i} \right) \right)^{2}} $$
Onde:<br>
$\hat{a}$ = Coeficiente angular da reta;<br>
$N$ = Número de elementos; <br>
$X$ = Valores do eixo das abcissas;<br>
$Y$ = Valores do eixo das ordenadas.<br>
</div>

### 4.2 Cálculo do Coeficiente Linear da Reta (b): <br>
$$ \hat{b} = \bar{Y_{i}} - \hat{a}\cdot \bar{X_{i}} $$
Onde:<br>
$\hat{b}$ = Coeficiente linear da reta;<br>
$\hat{a}$ = Coeficiente angular da reta;<br>
$\bar{X_{i}}$ = Média aritimética dos valores de X;<br>
$\bar{Y_{i}}$ = Média aritimética dos valores de Y.

### 4.3 Números aleatórios
<div style="text-align: justify">
Outra forma de obter os valores dos coeficientes se dá pela geração de números aleatórios. Em resumo, gerei um array de n números hipotéticos para possíveis valores de coeficientes angulares e apliquei a função para encontrar a norma de cada um deles, então, para o melhor resultado assumo que este será meu coeficiente angular.
</div> 

## 4.Conclusão
<div style="text-align: justify">
Na primeira parte do estudo, foi feita uma montagem bastante aprofundada para cada uma das cidades, no entanto, não foram plotadas e geradas todas as possíveis retas em função dos mais diversos períodos, com seus respectivos ajustes e coeficientes, até por que, seriam possíveis infinitas alternativas, no entanto, ficou bastante pronto para que qualquer análise requerida para avaliar os preços sejam promovidas.
Desta forma, a análise dos preços se deu de uma forma exploratória, abordando a cidade de Moscow, em todos os períodos existentes no data set.<br>
Os valores do dataset do desafio plotados formaram um gráfico de linha muito semelhante a uma reta, isso se deve ao fato de que o comportamento das variáveis serem semi-lineares, isto é, a medida que aumenta o diâmetro, aumenta o peso, com isso, a reta obtida foi bastante fiél com os dados.<br>
Por fim, gostaria de externar que o aprendizado foi de extrema qualiadade, já havia utilizado as bibliotecas do presente projeto em outros projetos acadêmicos, no entanto, consolidei ainda mais o conhecimento já existente e aprofundei muito mais em funções que não conhecia, o desenvolvimento do racicíonio para gerar o loop que encontra os valores Nans foi motivo de muito orgulho. Além do mais, pratiquei muito a escrita utilizando LateX que com certeza aprimorou muito a qualidade de leitura e compreendimento do projeto.
</div>
