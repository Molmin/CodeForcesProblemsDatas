## Description

<div><p>Vova has won $n$ trophies in different competitions. Each trophy is either golden or silver. The trophies are arranged in a row.</p><p>The <span class="tex-font-style-it">beauty</span> of the arrangement is the length of the longest subsegment consisting of golden trophies. Vova wants to swap two trophies (not necessarily adjacent ones) to make the arrangement as beautiful as possible — that means, to maximize the length of the longest such subsegment.</p><p>Help Vova! Tell him the maximum possible beauty of the arrangement if he is allowed to do at most one swap.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 10^5$) — the number of trophies.</p><p>The second line contains $n$ characters, each of them is either <span class="tex-font-style-tt">G</span> or <span class="tex-font-style-tt">S</span>. If the $i$-th character is <span class="tex-font-style-tt">G</span>, then the $i$-th trophy is a golden one, otherwise it's a silver trophy. </p></div><div class="output-specification"><p>Print the maximum possible length of a subsegment of golden trophies, if Vova is allowed to do at most one swap.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 10^5$) — the number of trophies.</p><p>The second line contains $n$ characters, each of them is either <span class="tex-font-style-tt">G</span> or <span class="tex-font-style-tt">S</span>. If the $i$-th character is <span class="tex-font-style-tt">G</span>, then the $i$-th trophy is a golden one, otherwise it's a silver trophy. </p>

## Output

<p>Print the maximum possible length of a subsegment of golden trophies, if Vova is allowed to do at most one swap.</p>





```input1
10
GGGSGGGSGG
```




```input2
4
GGGG
```




```input3
3
SSS
```




```output1
7
```




```output2
4
```




```output3
0
```



## Note

<p>In the first example Vova has to swap trophies with indices $4$ and $10$. Thus he will obtain the sequence "<span class="tex-font-style-tt">GGGGGGGSGS</span>", the length of the longest subsegment of golden trophies is $7$. </p><p>In the second example Vova can make no swaps at all. The length of the longest subsegment of golden trophies in the sequence is $4$. </p><p>In the third example Vova cannot do anything to make the length of the longest subsegment of golden trophies in the sequence greater than $0$.</p>
