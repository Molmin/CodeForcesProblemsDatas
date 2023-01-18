## Description

<div><p>The circle line of the Roflanpolis subway has $n$ stations.</p><p>There are two parallel routes in the subway. The first one visits stations in order $1 \to 2 \to \ldots \to n \to 1 \to 2 \to \ldots$ (so the next stop after station $x$ is equal to $(x+1)$ if $x &lt; n$ and $1$ otherwise). The second route visits stations in order $n \to (n-1) \to \ldots \to 1 \to n \to (n-1) \to \ldots$ (so the next stop after station $x$ is equal to $(x-1)$ if $x&gt;1$ and $n$ otherwise). All trains depart their stations simultaneously, and it takes exactly $1$ minute to arrive at the next station.</p><p>Two toads live in this city, their names are Daniel and Vlad.</p><p>Daniel is currently in a train of the <span class="tex-font-style-bf">first</span> route at station $a$ and will exit the subway when his train reaches station $x$.</p><p>Coincidentally, Vlad is currently in a train of the <span class="tex-font-style-bf">second</span> route at station $b$ and he will exit the subway when his train reaches station $y$.</p><p>Surprisingly, all numbers $a,x,b,y$ are distinct.</p><p>Toad Ilya asks you to check if Daniel and Vlad will ever be at the same station at the same time during their journey. In other words, check if there is a moment when their trains stop at the same station. Note that this includes the moments when Daniel or Vlad enter or leave the subway.</p></div><div class="input-specification"><p>The first line contains five space-separated integers $n$, $a$, $x$, $b$, $y$ ($4 \leq n \leq 100$, $1 \leq a, x, b, y \leq n$, all numbers among $a$, $x$, $b$, $y$ are distinct)&nbsp;— the number of stations in Roflanpolis, Daniel's start station, Daniel's finish station, Vlad's start station and Vlad's finish station, respectively.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">YES</span>" if there is a time moment when Vlad and Daniel are at the same station, and "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains five space-separated integers $n$, $a$, $x$, $b$, $y$ ($4 \leq n \leq 100$, $1 \leq a, x, b, y \leq n$, all numbers among $a$, $x$, $b$, $y$ are distinct)&nbsp;— the number of stations in Roflanpolis, Daniel's start station, Daniel's finish station, Vlad's start station and Vlad's finish station, respectively.</p>

## Output

<p>Output "<span class="tex-font-style-tt">YES</span>" if there is a time moment when Vlad and Daniel are at the same station, and "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each letter in any case (upper or lower).</p>





```input1
5 1 4 3 2
```




```input2
10 2 1 9 10
```




```output1
YES
```




```output2
NO
```



## Note

<p>In the first example, Daniel and Vlad start at the stations $(1, 3)$. One minute later they are at stations $(2, 2)$. They are at the same station at this moment. Note that Vlad leaves the subway right after that.</p><p>Consider the second example, let's look at the stations Vlad and Daniel are at. They are: </p><ul> <li> initially $(2, 9)$, </li><li> after $1$ minute $(3, 8)$, </li><li> after $2$ minutes $(4, 7)$, </li><li> after $3$ minutes $(5, 6)$, </li><li> after $4$ minutes $(6, 5)$, </li><li> after $5$ minutes $(7, 4)$, </li><li> after $6$ minutes $(8, 3)$, </li><li> after $7$ minutes $(9, 2)$, </li><li> after $8$ minutes $(10, 1)$, </li><li> after $9$ minutes $(1, 10)$. </li></ul><p>After that, they both leave the subway because they are at their finish stations, so there is no moment when they both are at the same station.</p>
