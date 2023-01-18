## Description

<div><p>You are a rebel leader and you are planning to start a revolution in your country. But the evil Government found out about your plans and set your punishment in the form of correctional labor.</p><p>You must paint a fence which consists of $10^{100}$ planks in two colors in the following way (suppose planks are numbered from left to right from $0$): </p><ul> <li> if the index of the plank is divisible by $r$ (such planks have indices $0$, $r$, $2r$ and so on) then you must paint it red; </li><li> if the index of the plank is divisible by $b$ (such planks have indices $0$, $b$, $2b$ and so on) then you must paint it blue; </li><li> if the index is divisible both by $r$ and $b$ <span class="tex-font-style-bf">you can choose the color</span> to paint the plank; </li><li> otherwise, you don't need to paint the plank at all (and it is forbidden to spent paint on it). </li></ul><p>Furthermore, the Government added one additional restriction to make your punishment worse. Let's list all <span class="tex-font-style-bf">painted</span> planks of the fence in ascending order: if there are $k$ consecutive planks with the same color in this list, then the Government will state that you failed the labor and execute you immediately. If you don't paint the fence according to the four aforementioned conditions, you will also be executed.</p><p>The question is: will you be able to accomplish the labor (the time is not important) or the execution is unavoidable and you need to escape at all costs.</p></div><div class="input-specification"><p>The first line contains single integer $T$ ($1 \le T \le 1000$) — the number of test cases.</p><p>The next $T$ lines contain descriptions of test cases — one per line. Each test case contains three integers $r$, $b$, $k$ ($1 \le r, b \le 10^9$, $2 \le k \le 10^9$) — the corresponding coefficients.</p></div><div class="output-specification"><p>Print $T$ words — one per line. For each test case print <span class="tex-font-style-tt">REBEL</span> (case insensitive) if the execution is unavoidable or <span class="tex-font-style-tt">OBEY</span> (case insensitive) otherwise.</p></div>

## Input

<p>The first line contains single integer $T$ ($1 \le T \le 1000$) — the number of test cases.</p><p>The next $T$ lines contain descriptions of test cases — one per line. Each test case contains three integers $r$, $b$, $k$ ($1 \le r, b \le 10^9$, $2 \le k \le 10^9$) — the corresponding coefficients.</p>

## Output

<p>Print $T$ words — one per line. For each test case print <span class="tex-font-style-tt">REBEL</span> (case insensitive) if the execution is unavoidable or <span class="tex-font-style-tt">OBEY</span> (case insensitive) otherwise.</p>





```input1
4
1 1 2
2 10 4
5 2 3
3 2 2
```




```output1
OBEY
REBEL
OBEY
OBEY
```


