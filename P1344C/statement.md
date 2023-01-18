## Description

<div><p>Logical quantifiers are very useful tools for expressing claims about a set. For this problem, let's focus on the set of real numbers specifically. <span class="tex-font-style-bf">The set of real numbers includes zero and negatives.</span> There are two kinds of quantifiers: universal ($\forall$) and existential ($\exists$). You can read more about them <a href="https://en.wikipedia.org/wiki/Quantifier_(logic)">here</a>.</p><p>The universal quantifier is used to make a claim that a statement holds <span class="tex-font-style-it">for all real numbers</span>. For example:</p><ul> <li> $\forall x,x&lt;100$ is read as: for all real numbers $x$, $x$ is less than $100$. This statement is false. </li><li> $\forall x,x&gt;x-1$ is read as: for all real numbers $x$, $x$ is greater than $x-1$. This statement is true. </li></ul><p>The existential quantifier is used to make a claim that <span class="tex-font-style-it">there exists some real number</span> for which the statement holds. For example:</p><ul> <li> $\exists x,x&lt;100$ is read as: there exists a real number $x$ such that $x$ is less than $100$. This statement is true. </li><li> $\exists x,x&gt;x-1$ is read as: there exists a real number $x$ such that $x$ is greater than $x-1$. This statement is true. </li></ul><p>Moreover, these quantifiers can be nested. For example:</p><ul> <li> $\forall x,\exists y,x&lt;y$ is read as: for all real numbers $x$, there exists a real number $y$ such that $x$ is less than $y$. This statement is true since for every $x$, there exists $y=x+1$. </li><li> $\exists y,\forall x,x&lt;y$ is read as: there exists a real number $y$ such that for all real numbers $x$, $x$ is less than $y$. This statement is false because it claims that there is a maximum real number: a number $y$ larger than every $x$. </li></ul><p><span class="tex-font-style-bf">Note that the order of variables and quantifiers is important for the meaning and veracity of a statement.</span></p><p>There are $n$ variables $x_1,x_2,\ldots,x_n$, and you are given some formula of the form $$ f(x_1,\dots,x_n):=(x_{j_1}&lt;x_{k_1})\land (x_{j_2}&lt;x_{k_2})\land \cdots\land (x_{j_m}&lt;x_{k_m}), $$</p><p>where $\land$ denotes logical AND. That is, $f(x_1,\ldots, x_n)$ is true if every inequality $x_{j_i}&lt;x_{k_i}$ holds. Otherwise, if at least one inequality does not hold, then $f(x_1,\ldots,x_n)$ is false.</p><p>Your task is to assign quantifiers $Q_1,\ldots,Q_n$ to either universal ($\forall$) or existential ($\exists$) so that the statement $$ Q_1 x_1, Q_2 x_2, \ldots, Q_n x_n, f(x_1,\ldots, x_n) $$</p><p>is true, and <span class="tex-font-style-bf">the number of universal quantifiers is maximized</span>, or determine that the statement is false for every possible assignment of quantifiers.</p><p><span class="tex-font-style-bf">Note that the order the variables appear in the statement is fixed.</span> For example, if $f(x_1,x_2):=(x_1&lt;x_2)$ then you are not allowed to make $x_2$ appear first and use the statement $\forall x_2,\exists x_1, x_1&lt;x_2$. If you assign $Q_1=\exists$ and $Q_2=\forall$, it will <span class="tex-font-style-bf">only</span> be interpreted as $\exists x_1,\forall x_2,x_1&lt;x_2$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2\le n\le 2\cdot 10^5$; $1\le m\le 2\cdot 10^5$)&nbsp;— the number of variables and the number of inequalities in the formula, respectively.</p><p>The next $m$ lines describe the formula. The $i$-th of these lines contains two integers $j_i$,$k_i$ ($1\le j_i,k_i\le n$, $j_i\ne k_i$).</p></div><div class="output-specification"><p>If there is no assignment of quantifiers for which the statement is true, output a single integer $-1$.</p><p>Otherwise, on the first line output an integer, the maximum possible number of universal quantifiers.</p><p>On the next line, output a string of length $n$, where the $i$-th character is "<span class="tex-font-style-tt">A</span>" if $Q_i$ should be a universal quantifier ($\forall$), or "<span class="tex-font-style-tt">E</span>" if $Q_i$ should be an existential quantifier ($\exists$). All letters should be upper-case. If there are multiple solutions where the number of universal quantifiers is maximum, print any.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2\le n\le 2\cdot 10^5$; $1\le m\le 2\cdot 10^5$)&nbsp;— the number of variables and the number of inequalities in the formula, respectively.</p><p>The next $m$ lines describe the formula. The $i$-th of these lines contains two integers $j_i$,$k_i$ ($1\le j_i,k_i\le n$, $j_i\ne k_i$).</p>

## Output

<p>If there is no assignment of quantifiers for which the statement is true, output a single integer $-1$.</p><p>Otherwise, on the first line output an integer, the maximum possible number of universal quantifiers.</p><p>On the next line, output a string of length $n$, where the $i$-th character is "<span class="tex-font-style-tt">A</span>" if $Q_i$ should be a universal quantifier ($\forall$), or "<span class="tex-font-style-tt">E</span>" if $Q_i$ should be an existential quantifier ($\exists$). All letters should be upper-case. If there are multiple solutions where the number of universal quantifiers is maximum, print any.</p>





```input1
2 1
1 2
```




```input2
4 3
1 2
2 3
3 1
```




```input3
3 2
1 3
2 3
```




```output1
1
AE
```




```output2
-1
```




```output3
2
AAE
```



## Note

<p>For the first test, the statement $\forall x_1, \exists x_2, x_1&lt;x_2$ is true. Answers of "<span class="tex-font-style-tt">EA</span>" and "<span class="tex-font-style-tt">AA</span>" give false statements. The answer "<span class="tex-font-style-tt">EE</span>" gives a true statement, but the number of universal quantifiers in this string is less than in our answer.</p><p>For the second test, we can show that no assignment of quantifiers, for which the statement is true exists.</p><p>For the third test, the statement $\forall x_1, \forall x_2, \exists x_3, (x_1&lt;x_3)\land (x_2&lt;x_3)$ is true: We can set $x_3=\max\{x_1,x_2\}+1$.</p>
