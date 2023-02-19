## Description

<div><p><span class="tex-font-style-it">No matter what trouble you're in, don't be afraid, but face it with a smile.</span></p><p><span class="tex-font-style-it">I've made another billion dollars!</span></p><p><span class="tex-font-style-it">&nbsp;— Boboniu</span></p><p>Boboniu has issued his currencies, named Bobo Yuan. Bobo Yuan (BBY) is a series of currencies. Boboniu gives each of them a positive integer identifier, such as BBY-1, BBY-2, etc.</p><p>Boboniu has a BBY collection. His collection looks like a sequence. For example:</p><center> <img class="tex-graphics" src="file://ADgCBISd.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>We can use sequence $a=[1,2,3,3,2,1,4,4,1]$ of length $n=9$ to denote it.</p><p>Now Boboniu wants to <span class="tex-font-style-it">fold</span> his collection. You can imagine that Boboniu stick his collection to a long piece of paper and fold it between currencies:</p><center> <img class="tex-graphics" src="file://xEXQsW7W.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Boboniu will only fold the same identifier of currencies together. In other words, if $a_i$ is folded over $a_j$ ($1\le i,j\le n$), then $a_i=a_j$ must hold. Boboniu doesn't care if you follow this rule in the process of folding. But once it is finished, the rule should be obeyed.</p><p>A formal definition of <span class="tex-font-style-it">fold</span> is described in notes.</p><p>According to the picture above, you can <span class="tex-font-style-it">fold</span> $a$ two times. In fact, you can <span class="tex-font-style-it">fold</span> $a=[1,2,3,3,2,1,4,4,1]$ at most two times. So the maximum number of folds of it is $2$.</p><p>As an international fan of Boboniu, you're asked to calculate the maximum number of folds. </p><p>You're given a sequence $a$ of length $n$, for each $i$ ($1\le i\le n$), you need to calculate the maximum number of folds of $[a_1,a_2,\ldots,a_i]$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1\le n\le 10^5$).</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\le a_i\le n$).</p></div><div class="output-specification"><p>Print $n$ integers. The $i$-th of them should be equal to the maximum number of folds of $[a_1,a_2,\ldots,a_i]$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1\le n\le 10^5$).</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\le a_i\le n$).</p>

## Output

<p>Print $n$ integers. The $i$-th of them should be equal to the maximum number of folds of $[a_1,a_2,\ldots,a_i]$.</p>





```input1
9
1 2 3 3 2 1 4 4 1
```




```input2
9
1 2 2 2 2 1 1 2 2
```




```input3
15
1 2 3 4 5 5 4 3 2 2 3 4 4 3 6
```




```input4
50
1 2 4 6 6 4 2 1 3 5 5 3 1 2 4 4 2 1 3 3 1 2 2 1 1 1 2 4 6 6 4 2 1 3 5 5 3 1 2 4 4 2 1 3 3 1 2 2 1 1
```




```output1
0 0 0 1 1 1 1 2 2
```




```output2
0 0 1 2 3 3 4 4 5
```




```output3
0 0 0 0 0 1 1 1 1 2 2 2 3 3 0
```




```output4
0 0 0 0 1 1 1 1 1 1 2 2 2 2 2 3 3 3 3 4 4 4 5 5 6 7 3 3 3 4 4 4 4 3 3 4 4 4 4 4 5 5 5 5 6 6 6 7 7 8
```



## Note

<p>Formally, for a sequence $a$ of length $n$, let's define the <span class="tex-font-style-it">folding sequence</span> as a sequence $b$ of length $n$ such that:</p><ul> <li> $b_i$ ($1\le i\le n$) is either $1$ or $-1$. </li><li> Let $p(i)=[b_i=1]+\sum_{j=1}^{i-1}b_j$. For all $1\le i&lt;j\le n$, if $p(i)=p(j)$, then $a_i$ should be equal to $a_j$. </li></ul><p>($[A]$ is the value of boolean expression $A$. i. e. $[A]=1$ if $A$ is true, else $[A]=0$).</p><p>Now we define the number of folds of $b$ as $f(b)=\sum_{i=1}^{n-1}[b_i\ne b_{i+1}]$.</p><p>The maximum number of folds of $a$ is $F(a)=\max\{ f(b)\mid b \text{ is a folding sequence of }a \}$.</p>
