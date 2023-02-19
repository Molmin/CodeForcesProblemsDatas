## Description

<div><p>Helen studies functional programming and she is fascinated with a concept of <span class="tex-font-style-underline">higher order functions</span>&nbsp;— functions that are taking other functions as parameters. She decides to generalize the concept of the function <span class="tex-font-style-underline">order</span> and to test it on some examples. </p><p>For her study, she defines a simple grammar of types. In her grammar, a type non-terminal $T$ is defined as one of the following grammar productions, together with $\textrm{order}(T)$, defining an order of the corresponding type:</p><ul><li> "<span class="tex-font-style-tt">()</span>" is a unit type, $\textrm{order}(\textrm{"}\texttt{()}\textrm{"}) = 0$.</li><li> "(" $T$ ")" is a parenthesized type, $\textrm{order}(\textrm{"}\texttt{(}\textrm{"}\,T\,\textrm{"}\texttt{)}\textrm{"}) = \textrm{order}(T)$.</li><li> $T_1$ "<span class="tex-font-style-tt">-&gt;</span>" $T_2$ is a functional type, $\textrm{order}(T_1\,\textrm{"}\texttt{-&gt;}\textrm{"}\,T_2) = max(\textrm{order}(T_1) + 1, \textrm{order}(T_2))$. The function constructor $T_1$ "<span class="tex-font-style-tt">-&gt;</span>" $T_2$ is right-to-left associative, so the type "<span class="tex-font-style-tt">()-&gt;()-&gt;()</span>" is the same as the type "<span class="tex-font-style-tt">()-&gt;(()-&gt;())</span>" of a function returning a function, and it has an order of $1$. While "<span class="tex-font-style-tt">(()-&gt;())-&gt;()</span>" is a function that has an order-1 type "<span class="tex-font-style-tt">(()-&gt;())</span>" as a parameter, and it has an order of $2$. </li></ul> <p>Helen asks for your help in writing a program that computes an order of the given type.</p></div><div class="input-specification"><p>The single line of the input contains a string consisting of characters '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>', '<span class="tex-font-style-tt">-</span>', and '<span class="tex-font-style-tt">&gt;</span>' that describes a type that is valid according to the grammar from the problem statement. The length of the line is at most $10^4$ characters.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the order of the given type.</p></div>

## Input

<p>The single line of the input contains a string consisting of characters '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>', '<span class="tex-font-style-tt">-</span>', and '<span class="tex-font-style-tt">&gt;</span>' that describes a type that is valid according to the grammar from the problem statement. The length of the line is at most $10^4$ characters.</p>

## Output

<p>Print a single integer&nbsp;— the order of the given type.</p>





```input1
()
```




```input2
()-&gt;()
```




```input3
()-&gt;()-&gt;()
```




```input4
(()-&gt;())-&gt;()
```




```input5
()-&gt;(((()-&gt;())-&gt;()-&gt;())-&gt;())
```




```output1
0
```




```output2
1
```




```output3
1
```




```output4
2
```




```output5
3
```


