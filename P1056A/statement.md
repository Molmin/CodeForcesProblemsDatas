## Description

<div><p>Arkady's morning seemed to be straight of his nightmare. He overslept through the whole morning and, still half-asleep, got into the tram that arrived the first. Some time after, leaving the tram, he realized that he was not sure about the line number of the tram he was in.</p><p>During his ride, Arkady woke up several times and each time he saw the tram stopping at some stop. For each stop he knows which lines of tram stop there. Given this information, can you help Arkady determine what are the possible lines of the tram he was in?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 100$)&nbsp;— the number of stops Arkady saw.</p><p>The next $n$ lines describe the stops. Each of them starts with a single integer $r$ ($1 \le r \le 100$)&nbsp;— the number of tram lines that stop there. $r$ distinct integers follow, each one between $1$ and $100$, inclusive,&nbsp;— the line numbers. They can be in arbitrary order.</p><p>It is guaranteed that Arkady's information is consistent, i.e. there is at least one tram line that Arkady could take.</p></div><div class="output-specification"><p>Print all tram lines that Arkady could be in, in arbitrary order.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 100$)&nbsp;— the number of stops Arkady saw.</p><p>The next $n$ lines describe the stops. Each of them starts with a single integer $r$ ($1 \le r \le 100$)&nbsp;— the number of tram lines that stop there. $r$ distinct integers follow, each one between $1$ and $100$, inclusive,&nbsp;— the line numbers. They can be in arbitrary order.</p><p>It is guaranteed that Arkady's information is consistent, i.e. there is at least one tram line that Arkady could take.</p>

## Output

<p>Print all tram lines that Arkady could be in, in arbitrary order.</p>





```input1
3
3 1 4 6
2 1 4
5 10 5 6 4 1
```




```input2
5
1 1
10 10 9 8 7 100 5 4 3 99 1
5 1 2 3 4 5
5 4 1 3 2 5
4 10 1 5 3
```




```output1
1 4
```




```output2
1
```



## Note

<p>Consider the first example. Arkady woke up three times. The first time he saw a stop with lines $1$, $4$, $6$. The second time he saw a stop with lines $1$, $4$. The third time he saw a stop with lines $10$, $5$, $6$, $4$ and $1$. He can be in a tram of one of two lines: $1$ or $4$.</p>
