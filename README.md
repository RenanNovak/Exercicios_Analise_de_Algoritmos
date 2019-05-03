# Exercícios - Análise de Algoritmos

**1. Quais são as duas características mais comuns para analisar algoritmos?**

As duas características mais comuns para analisar um software para dizer se é bom ou ruim são: Tempo e Consumo de memória.

&nbsp;

**2. Por que a medida de tempo em segundos não representa qualificadamente o tempo de execução de um algoritmo?**

Não é medida em tempo o software já que deve possuir certa independência entre a tecnología; o software e o hardware.

&nbsp;

**3. A medida de tempo de um algoritmo é realizada através de qual informação? O que pode afetá-la?**

A medição do tempo em representação a qualidade e estabilidade do software é feita mediante os passos do algoritmo que precisa para finalizar a sua execução.
Pode afetá-la pelo ambiente do hardware em que ela é executada e o tamanho da entrada.

&nbsp;

**4. Na análise de algoritmos, qual é o valor da base da função logarítmica e exponencial? Por que é escolhido este valor?**

A base da função logarítmica e exponencial é 2.
A base 2 tem uma importância muito considerada na informática dada a codificação binária que utiliza. O número determinado em um bit é de oito (8) exemplares que podem codificar-se com 2^8 = 256 que é o número de variações que pode realizar-se.
O algoritmo binário tem uma frequência de aparição grande no análise de algoritmos.

&nbsp;

**5. O que é complexidade de tempo?**

É uma função que representa o número máximo de passos de um algoritmo.

&nbsp;

**6. Dado dois algoritmos A e B com as complexidades de tempo respectivamente *f*1 e *f*2, qual é o melhor algoritmo? O que indica qual é o melhor algoritmo?**

Considerando A e B dois algoritmos totalmentes diferentes, é selecionado o melhor aquele que é executado com menores números de passos à finalização da execução e aquele que tem uma menor complexidade de tempo. Sendo o melhor o *f*1, pois tem a menor entrada

&nbsp;

**7. Em uma função de complexidade, o que representa o termo *n*?**

Em uma função de complexidade o termo “n” é considerado como o comprimento da entrada.

&nbsp;

**8. Quais são as operações primitivas de um algoritmo?**

As operações primitivas de um algoritmo são:
<p>
·        Atribuição de valores a variáveis;<br>
·        Chamadas de métodos;<br>
·        Operações aritméticas;<br>
·        Comparação de dois números;<br>
·        Acesso a um arranjo;<br>
·        Seguimento de uma referência para um objeto;<br>
·        Retorno de um método.<br>

&nbsp;

**9. Qual é o valor de uma operação primitiva de um algoritmo?**

Para cada valor de uma operação primitiva de um algoritmo é atribuído o valor 1.

&nbsp;

**10. Desenvolva o pseudocódigo do algoritmo SOMA, que realiza a soma de dois números inteiros recebidos por parâmetro e tem como saída a resultado da operação. Identifique a sua função de complexidade de tempo.**

1 - p <- a + b<br>
2 - retorna p;<br>
<br>
Sendo custo c1 e c2; <br>
f(n) = c1 . 1 + c2 . 1 <br>
f(n) = 1 + 1 <br>
f(n) = 2

&nbsp;

**11. Desenvolva o pseudocódigo do algoritmo SOMA_VETOR, que realiza a soma de todos os elementos de um vetor. O algoritmo recebe o vetor V e tem como saída o resultado. Identifique a sua função de complexidade de tempo.**

1 - soma <- 0;<br>
2 - N <- comprimento V;<br>
3 - para i <- 1 até N:<br>
4 -        soma <- soma + V[i]<br>
5 -        i <- i + 1<br>
6 - retorna soma;<br>
<br>
Sendo custo c1, c2, c3, c4, c5 e c6, o número de vezes no para(for) assume o valor de n, então: <br>
f(n) = c1 . 1 + c2 . 1 + c3 . n + c4 . n + c5 . n + c6 . 1 <br>
f(n) = 1 + 1 + n + n + n + 1 <br>
f(n) = 3n + 3

&nbsp;

**12. Desenvolva o pseudocódigo do algoritmo CONTAGEM_IMPARES, que realiza a contagem de números impares de um vetor. O algoritmo recebe o vetor V e tem como saída o resultado. Identifique a sua função de complexidade de tempo.**

1 - cont <- 0;<br>
2 - N < comprimento V;<br>
3 - para i <- 1 até N:<br>
4 -        se V[i]%2 != 0:<br>
5 -           cont <- cont + 1<br>
7 -        i <- i + 1<br>
8 - retorna cont;<br>
<br>
Sendo custo c1, c2, c3, c4, c5, c6 e c7, o número de vezes no para(for) e se(if) assume o valor de n, então: <br>
f(n) = c1 . 1 + c2 . 1 + c3 . n + c4 . n + c5 . n + c6 . n + c7 . 1 <br>
f(n) = 1 + 1 + n + n + n + n + 1 <br>
f(n) = 4n + 3

&nbsp;

**13. Desenvolva o pseudocódigo do algoritmo SOMA_MATRIZ, que realiza a soma de todos os elementos de uma matriz. O algoritmo recebe a matriz M e tem como saída o resultado. Identifique a sua função de complexidade de tempo.**

1 - soma <- 0;<br>
2 - N <- comprimento M;<br>
3 - para i <- até N:<br>
4 -        para j <- 1 até N:<br>
5 -             soma <- soma + M[i][j]<br>
6 -             j <- j + 1<br>
7 -        i <- i + 1<br>
8 - retorna soma;<br>
<br>
Sendo custo c1, c2, c3, c4, c5, c6, c7 e c8, o número de vezes no para(for) assume o valor de n, para o para(for) dentro do outro para(for), o número de vezes assume o valor de n . n, então: <br>
f(n) = 1 + 1 + n + n * n + n * n + n * n + n + 1 <br>
f(n) = 3n² + 2n + 3

&nbsp;

**14. Desenvolva o pseudocódigo do algoritmo BUSCA_MATRIZ, que identifica posição x e y de um elemento em uma matriz. O algoritmo recebe a matriz M e o valor V e tem como saída a posição x e y. Identifique a sua função de complexidade de tempo.**

1 - N <- comprimento M;<br>
2 - para i <- 1 até N:<br>
3 -        para j <- 1 até N:<br>
4 -             se M[i][j] = V:<br>
5 -                retorna M[i][j];<br>
6 -             j <- j + 1<br>
7 -        i <- i + 1<br>
8 - retorna M;<br>
<br>
Sendo custo c1, c2, c3, c4, c5, c6, c7 e c8, o número de vezes no para(for) assume o valor de n, para o para(for) dentro do outro para(for) e o se(if), o número de vezes assume o valor de n . n, então: <br>
f(n) = 1 + n + n² + n² + n² + n² + n + 1 <br>
f(n) = 4n² + 2n + 2

&nbsp;

**15. O que é análise assintótica? Qual é o seu objetivo?**

Objetivo de compreender o tempo de execução para entradas grandes. Ou seja, é um método de descrever o comportamento de limites.

&nbsp;

**16. Qual é o processo da análise assintótica? Crie um exemplo.**

![](https://github.com/RenanNovak/Exercicios_Analise_de_Algoritmos/blob/master/img/img16.jpg)

&nbsp;

**17. O que é notação assintótica?**

Queremos saber é quanto tempo esses algoritmos demoram. Estamos interessados no tempo, não só nas suposições. Os tempos de execução da busca linear e da busca binária incluem o tempo necessário para gerar e checar palpites.
O tempo de execução de um algoritmo depende do quão demorado é para um computador executar as linhas de código do algoritmo e isto depende da velocidade deste computador, da linguagem de programação, e do compilador que traduziu o programa da linguagem de programação para o código que executa diretamente no computador, entre outros fatores.

&nbsp;

**18. O que é notação O-Grande ou Big-Oh?**

A notação Big O é uma ferramenta específica para avaliar a eficiência do algoritmo. A notação Big O geralmente é usada para mostrar como os programas precisam de recursos em relação ao tamanho de entrada.
Usamos a notação big-Θ para delimitar assintoticamente o crescimento do tempo de execução dentro dos fatores constantes superiores e inferiores. Algumas vezes queremos saber apenas o limite superior. 

&nbsp;

**19. Qual é a definição formal da notação O-Grande?**

Notação O–grande diz que uma função é menor que ou igual a outra função g(n). x Ou seja, f é limitada superiormente por g (até no máximo um fator constante) assintoticamente.

&nbsp;

**20. Crie um gráfico explicando a notação O-Grande. Utilize f(n) = 2n + 4. Qual é um valor possível para n0?**

![](https://github.com/RenanNovak/Exercicios_Analise_de_Algoritmos/blob/master/img/img20.jpg)

N0 = 4

&nbsp;


**21. O que é a notação o-pequeno ou Little-Oh?**

É uma notação a qual diz que uma função é menor que a outra.

&nbsp;

**22. Qual é a definição formal da notação o-pequeno?**

Definição formal: f (n) = o (g (n)) significa que para todo c> 0 existe algum k> 0 tal que 0 ≤ f (n) <cg (n) para todo n ≥ k. O valor de k não deve depender de n, mas pode depender de c.
Onde R+ é o conjunto dos reais não negativos.

&nbsp;

**23. Crie um gráfico explicando a notação o-pequeno?**

![](https://github.com/RenanNovak/Exercicios_Analise_de_Algoritmos/blob/master/img/img23.jpg)

Notação O –pequeno diz que uma função é menor que a outra função g(n). Ou seja, f é dominada por g assintoticamente. A diferença entre Big-Oh e Little-Oh é análoga àquela entre ≤ e <.  

&nbsp;

**24. Passe a notação O-Grande e o-pequeno as funções abaixo:**

![](https://github.com/RenanNovak/Exercicios_Analise_de_Algoritmos/blob/master/img/img24.jpg)

&nbsp;

**25. Identifique o O-Grande dos algoritmos desenvolvidos nos problemas 10 até 14.**

10- f(n)=2 <br>
O = 1
<br><br>
11- f(n)=3n+3 <br>
O = n
<br><br>
12- f(n)=4n+3 <br>
O = n
<br><br>
13- f(n)=3n² + 2n + 3 <br>
O = n²
<br><br>
14- f(n)=4n² + 2n + 2 <br>
O = n²

&nbsp;
