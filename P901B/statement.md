## Description

<div><p>Suppose you have two polynomials <img align="middle" class="tex-formula" src="file://IqEKfS6w.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://slHgeZCE.png" style="max-width: 100.0%;max-height: 100.0%;">. Then polynomial <img align="middle" class="tex-formula" src="file://z1MXOiAB.png" style="max-width: 100.0%;max-height: 100.0%;"> can be uniquely represented in the following way:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://xBWVkrdT.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>This can be done using <a href="https://en.wikipedia.org/wiki/Polynomial_long_division">long division</a>. Here, <img align="middle" class="tex-formula" src="file://4Za95UlG.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the degree of polynomial <span class="tex-span"><i>P</i>(<i>x</i>)</span>. <img align="middle" class="tex-formula" src="file://m818BqFA.png" style="max-width: 100.0%;max-height: 100.0%;"> is called the remainder of division of polynomial <img align="middle" class="tex-formula" src="file://OJ0Nh8uI.png" style="max-width: 100.0%;max-height: 100.0%;"> by polynomial <img align="middle" class="tex-formula" src="file://QbZ3ClRN.png" style="max-width: 100.0%;max-height: 100.0%;">, it is also denoted as <img align="middle" class="tex-formula" src="file://Ewl990af.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>Since there is a way to divide polynomials with remainder, we can define Euclid's algorithm of finding the greatest common divisor of two polynomials. The algorithm takes two polynomials <img align="middle" class="tex-formula" src="file://AvtOmxZp.png" style="max-width: 100.0%;max-height: 100.0%;">. If the polynomial <img align="middle" class="tex-formula" src="file://ROQ0mNEr.png" style="max-width: 100.0%;max-height: 100.0%;"> is zero, the result is <img align="middle" class="tex-formula" src="file://zzWUl7JH.png" style="max-width: 100.0%;max-height: 100.0%;">, otherwise the result is the value the algorithm returns for pair <img align="middle" class="tex-formula" src="file://WNL2csVy.png" style="max-width: 100.0%;max-height: 100.0%;">. On each step the degree of the second argument decreases, so the algorithm works in finite number of steps. But how large that number could be? You are to answer this question. </p><p>You are given an integer <span class="tex-span"><i>n</i></span>. You have to build two polynomials with degrees not greater than <span class="tex-span"><i>n</i></span>, such that their coefficients are integers not exceeding <span class="tex-span">1</span> by their absolute value, the leading coefficients (ones with the greatest power of <span class="tex-span"><i>x</i></span>) are equal to one, and the described Euclid's algorithm performs exactly <span class="tex-span"><i>n</i></span> steps finding their greatest common divisor. Moreover, the degree of the first polynomial should be greater than the degree of the second. By a step of the algorithm we mean the transition from pair <img align="middle" class="tex-formula" src="file://l3Mn0bFT.png" style="max-width: 100.0%;max-height: 100.0%;"> to pair <img align="middle" class="tex-formula" src="file://N77n3bWC.png" style="max-width: 100.0%;max-height: 100.0%;">. </p></div><div class="input-specification"><p>You are given a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 150</span>)&nbsp;— the number of steps of the algorithm you need to reach.</p></div><div class="output-specification"><p>Print two polynomials in the following format.</p><p>In the first line print a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i></span>)&nbsp;— the degree of the polynomial. </p><p>In the second line print <span class="tex-span"><i>m</i> + 1</span> integers between <span class="tex-span"> - 1</span> and <span class="tex-span">1</span>&nbsp;— the coefficients of the polynomial, from constant to leading. </p><p>The degree of the first polynomial should be greater than the degree of the second polynomial, the leading coefficients should be equal to <span class="tex-span">1</span>. Euclid's algorithm should perform exactly <span class="tex-span"><i>n</i></span> steps when called using these polynomials.</p><p>If there is no answer for the given <span class="tex-span"><i>n</i></span>, print <span class="tex-font-style-tt">-1</span>.</p><p>If there are multiple answer, print any of them.</p></div>

## Input

<p>You are given a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 150</span>)&nbsp;— the number of steps of the algorithm you need to reach.</p>

## Output

<p>Print two polynomials in the following format.</p><p>In the first line print a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i></span>)&nbsp;— the degree of the polynomial. </p><p>In the second line print <span class="tex-span"><i>m</i> + 1</span> integers between <span class="tex-span"> - 1</span> and <span class="tex-span">1</span>&nbsp;— the coefficients of the polynomial, from constant to leading. </p><p>The degree of the first polynomial should be greater than the degree of the second polynomial, the leading coefficients should be equal to <span class="tex-span">1</span>. Euclid's algorithm should perform exactly <span class="tex-span"><i>n</i></span> steps when called using these polynomials.</p><p>If there is no answer for the given <span class="tex-span"><i>n</i></span>, print <span class="tex-font-style-tt">-1</span>.</p><p>If there are multiple answer, print any of them.</p>





```input1
1

```




```input2
2

```




```output1
1
0 1
0
1

```




```output2
2
-1 0 1
1
0 1

```



## Note

<p>In the second example you can print polynomials <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> - 1</span> and <span class="tex-span"><i>x</i></span>. The sequence of transitions is</p><center class="tex-equation"><span class="tex-span">(<i>x</i><sup class="upper-index">2</sup> - 1, <i>x</i>) → (<i>x</i>,  - 1) → ( - 1, 0).</span></center><p>There are two steps in it.</p>
