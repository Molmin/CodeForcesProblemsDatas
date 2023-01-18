## Description

<div><p><span class="tex-font-style-it">This is a harder version of the problem. In this version $n \le 500\,000$</span></p><p>The outskirts of the capital are being actively built up in Berland. The company "Kernel Panic" manages the construction of a residential complex of skyscrapers in New Berlskva. All skyscrapers are built along the highway. It is known that the company has already bought $n$ plots along the highway and is preparing to build $n$ skyscrapers, one skyscraper per plot.</p><p>Architects must consider several requirements when planning a skyscraper. Firstly, since the land on each plot has different properties, each skyscraper has a limit on the largest number of floors it can have. Secondly, according to the design code of the city, it is unacceptable for a skyscraper to simultaneously have higher skyscrapers both to the left and to the right of it.</p><p>Formally, let's number the plots from $1$ to $n$. Then if the skyscraper on the $i$-th plot has $a_i$ floors, it must hold that $a_i$ is at most $m_i$ ($1 \le a_i \le m_i$). Also there mustn't be integers $j$ and $k$ such that $j &lt; i &lt; k$ and $a_j &gt; a_i &lt; a_k$. Plots $j$ and $k$ are <span class="tex-font-style-bf">not</span> required to be adjacent to $i$.</p><p>The company wants the total number of floors in the built skyscrapers to be as large as possible. Help it to choose the number of floors for each skyscraper in an optimal way, i.e. in such a way that all requirements are fulfilled, and among all such construction plans choose any plan with the maximum possible total number of floors.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 500\,000$)&nbsp;— the number of plots.</p><p>The second line contains the integers $m_1, m_2, \ldots, m_n$ ($1 \leq m_i \leq 10^9$)&nbsp;— the limit on the number of floors for every possible number of floors for a skyscraper on each plot.</p></div><div class="output-specification"><p>Print $n$ integers $a_i$&nbsp;— the number of floors in the plan for each skyscraper, such that all requirements are met, and the total number of floors in all skyscrapers is the maximum possible.</p><p>If there are multiple answers possible, print any of them.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 500\,000$)&nbsp;— the number of plots.</p><p>The second line contains the integers $m_1, m_2, \ldots, m_n$ ($1 \leq m_i \leq 10^9$)&nbsp;— the limit on the number of floors for every possible number of floors for a skyscraper on each plot.</p>

## Output

<p>Print $n$ integers $a_i$&nbsp;— the number of floors in the plan for each skyscraper, such that all requirements are met, and the total number of floors in all skyscrapers is the maximum possible.</p><p>If there are multiple answers possible, print any of them.</p>





```input1
5
1 2 3 2 1

```




```input2
3
10 6 8

```




```output1
1 2 3 2 1 

```




```output2
10 6 6 

```



## Note

<p>In the first example, you can build all skyscrapers with the highest possible height.</p><p>In the second test example, you cannot give the maximum height to all skyscrapers as this violates the design code restriction. The answer $[10, 6, 6]$ is optimal. Note that the answer of $[6, 6, 8]$ also satisfies all restrictions, but is not optimal.</p>
