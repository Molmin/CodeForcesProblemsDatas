## Description

<div><p>C*++ language is quite similar to C++. The similarity manifests itself in the fact that the programs written in C*++ sometimes behave unpredictably and lead to absolutely unexpected effects. For example, let's imagine an arithmetic expression in C*++ that looks like this (<span class="tex-span"><i>expression</i></span> is the main term):</p><ul> <li> <span class="tex-span"><i>expression</i></span> ::= <span class="tex-span"><i>summand</i></span> | <span class="tex-span"><i>expression</i> + <i>summand</i></span> | <span class="tex-span"><i>expression</i> - <i>summand</i></span> </li><li> <span class="tex-span"><i>summand</i></span> ::= <span class="tex-span"><i>increment</i></span> | <span class="tex-span"><i>coefficient</i></span>*<span class="tex-span"><i>increment</i></span> </li><li> <span class="tex-span"><i>increment</i></span> ::= a++ | ++a </li><li> <span class="tex-span"><i>coefficient</i></span> ::= 0|1|2|...|1000 </li></ul><p>For example, "<span class="tex-font-style-tt">5*a++-3*++a+a++</span>" is a valid expression in C*++.</p><p>Thus, we have a sum consisting of several summands divided by signs "<span class="tex-font-style-tt">+</span>" or "<span class="tex-font-style-tt">-</span>". Every summand is an expression "<span class="tex-font-style-tt">a++</span>" or "<span class="tex-font-style-tt">++a</span>" multiplied by some integer coefficient. If the coefficient is omitted, it is suggested being equal to <span class="tex-span">1</span>.</p><p>The calculation of such sum in C*++ goes the following way. First all the summands are calculated one after another, then they are summed by the usual arithmetic rules. If the summand contains "<span class="tex-font-style-tt">a++</span>", then during the calculation first the value of the "<span class="tex-font-style-tt">a</span>" variable is multiplied by the coefficient, then value of "<span class="tex-font-style-tt">a</span>" is increased by <span class="tex-span">1</span>. If the summand contains "<span class="tex-font-style-tt">++a</span>", then the actions on it are performed in the reverse order: first "<span class="tex-font-style-tt">a</span>" is increased by <span class="tex-span">1</span>, then — multiplied by the coefficient.</p><p>The summands may be calculated in any order, that's why sometimes the result of the calculation is completely unpredictable! Your task is to find its largest possible value.</p></div><div class="input-specification"><p>The first input line contains an integer <span class="tex-span"><i>a</i></span> (<span class="tex-span"> - 1000 ≤ <i>a</i> ≤ 1000</span>) — the initial value of the variable "<span class="tex-font-style-tt">a</span>". The next line contains an expression in C*++ language of the described type. The number of the summands in the expression does not exceed <span class="tex-span">1000</span>. It is guaranteed that the line describing the expression contains no spaces and tabulation. </p></div><div class="output-specification"><p>Output a single number — the maximal possible value of the expression.</p></div>

## Input

<p>The first input line contains an integer <span class="tex-span"><i>a</i></span> (<span class="tex-span"> - 1000 ≤ <i>a</i> ≤ 1000</span>) — the initial value of the variable "<span class="tex-font-style-tt">a</span>". The next line contains an expression in C*++ language of the described type. The number of the summands in the expression does not exceed <span class="tex-span">1000</span>. It is guaranteed that the line describing the expression contains no spaces and tabulation. </p>

## Output

<p>Output a single number — the maximal possible value of the expression.</p>





```input1
1
5*a++-3*++a+a++

```




```input2
3
a+++++a

```




```output1
11

```




```output2
8

```



## Note

<p>Consider the second example. Initially <span class="tex-span"><i>a</i> = 3</span>. Suppose that at first the first summand is calculated, and then the second one is. The first summand gets equal to <span class="tex-span">3</span>, and the value of <span class="tex-span"><i>a</i></span> is increased by <span class="tex-span">1</span>. At the calculation of the second summand <span class="tex-span"><i>a</i></span> is increased once more (gets equal to <span class="tex-span">5</span>). The value of the second summand is <span class="tex-span">5</span>, and together they give <span class="tex-span">8</span>. If we calculate the second summand first and the first summand later, then the both summands equals to <span class="tex-span">4</span>, and the result is <span class="tex-span">8</span>, too.</p>
