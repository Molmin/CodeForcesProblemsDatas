## Description

<div><p>Let $f(x,y)$ be the number of <span class="tex-font-style-it">carries</span> of $x+y$ in binary (i.&nbsp;e. $f(x,y)=g(x)+g(y)-g(x+y)$, where $g(x)$ is the number of ones in the binary representation of $x$).</p><p>Given two integers $n$ and $k$, find the number of ordered pairs $(a,b)$ such that $0 \leq a,b &lt; 2^n$, and $f(a,b)$ equals $k$. Note that for $a\ne b$, $(a,b)$ and $(b,a)$ are considered as two different pairs. </p><p>As this number may be large, output it modulo $10^9+7$.</p></div><div class="input-specification"><p>The only line of each test contains two integers $n$ and $k$ ($0\leq k&lt;n\leq 10^6$).</p></div><div class="output-specification"><p>Output a single integer &nbsp;— the answer modulo $10^9+7$.</p></div>

## Input

<p>The only line of each test contains two integers $n$ and $k$ ($0\leq k&lt;n\leq 10^6$).</p>

## Output

<p>Output a single integer &nbsp;— the answer modulo $10^9+7$.</p>





```input1
3 1
```




```input2
3 0
```




```input3
998 244
```




```output1
15
```




```output2
27
```




```output3
573035660
```



## Note

<p>Here are some examples for understanding <span class="tex-font-style-it">carries</span>:</p><p>$$ \begin{aligned} &amp;\begin{array}{r} 1_{\ \ }1_{\ \ }1\\ +\ _{1}1_{\ \ }0_{\ \ }0\\ \hline \ 1_{\ \ }0_{\ \ }1_{\ \ }1 \end{array} &amp;\begin{array}{r} \ 1_{\ \ }0_{\ \ }1\\ +\ _{\ \ }0_{\ \ }0_{1}1\\ \hline \ 0_{\ \ }1_{\ \ }1_{\ \ }0 \end{array} &amp; &amp;\begin{array}{r} \ 1_{\ \ }0_{\ \ }1\\ +\ _{1}0_{1}1_{1}1\\ \hline \ 1_{\ \ }0_{\ \ }0_{\ \ }0 \end{array} \end{aligned} $$</p><p>So $f(7,4)=1$, $f(5,1)=1$ and $f(5,3)=3$.</p><p>In the first test case, all the pairs meeting the constraints are $(1,1),(1,5),(2,2),(2,3),(3,2),(4,4),(4,5),(4,6),(4,7),(5,1),(5,4),(5,6),(6,4),(6,5),(7,4)$.</p>
