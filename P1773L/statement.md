## Description

<div><p>Lisa loves playing with the sequences of integers. When she gets a new integer sequence $a_i$ of length $n$, she starts looking for all <span class="tex-font-style-it">monotone</span> subsequences. A monotone subsequence $[l, r]$ is defined by two indices $l$ and $r$ ($1 \le l &lt; r \le n$) such that $\forall i = l, l+1, \ldots, r-1: a_i \le a_{i+1}$ or $\forall i = l, l+1, \ldots, r-1: a_i \ge a_{i+1}$. </p><p>Lisa considers a sequence $a_i$ to be <span class="tex-font-style-it">boring</span> if there is a monotone subsequence $[l, r]$ that is as long as her boredom threshold $k$, that is when $r - l + 1 = k$.</p><p>Lucas has a sequence $b_i$ that he wants to present to Lisa, but the sequence might be boring for Lisa. So, he wants to change some elements of his sequence $b_i$, so that Lisa does not get bored playing with it. However, Lucas is lazy and wants to change as few elements of the sequence $b_i$ as possible. Your task is to help Lucas find the required changes. </p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($3 \le k \le n \le 10^6$)&nbsp;— the length of the sequence and Lisa's boredom threshold. The second line contains $n$ integers $b_i$ ($1 \le b_i \le 99\,999$)&nbsp;— the original sequence that Lucas has.</p></div><div class="output-specification"><p>On the first line output an integer $m$&nbsp;— the minimal number of elements in $b_i$ that needs to be changed to make the sequence not boring for Lisa. On the second line output $n$ integers $a_i$ ($0 \le a_i \le 100\,000$), so that the sequence of integers $a_i$ is not boring for Lisa and is different from the original sequence $b_i$ in exactly $m$ positions.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($3 \le k \le n \le 10^6$)&nbsp;— the length of the sequence and Lisa's boredom threshold. The second line contains $n$ integers $b_i$ ($1 \le b_i \le 99\,999$)&nbsp;— the original sequence that Lucas has.</p>

## Output

<p>On the first line output an integer $m$&nbsp;— the minimal number of elements in $b_i$ that needs to be changed to make the sequence not boring for Lisa. On the second line output $n$ integers $a_i$ ($0 \le a_i \le 100\,000$), so that the sequence of integers $a_i$ is not boring for Lisa and is different from the original sequence $b_i$ in exactly $m$ positions.</p>





```input1
5 3
1 2 3 4 5
```




```input2
6 3
1 1 1 1 1 1
```




```input3
6 4
1 1 4 4 1 1
```




```input4
6 4
4 4 4 2 2 2
```




```input5
6 4
4 4 4 3 4 4
```




```input6
8 4
2 1 1 3 3 1 1 2
```




```input7
10 4
1 1 1 2 2 1 1 2 2 1
```




```input8
7 5
5 4 4 3 4 4 4
```




```input9
10 10
1 1 1 1 1 1 1 1 1 1
```




```output1
2
1 0 3 0 5
```




```output2
3
1 100000 0 1 0 1
```




```output3
1
1 1 4 0 1 1
```




```output4
2
4 4 0 2 0 2
```




```output5
1
4 4 100000 3 4 4
```




```output6
2
2 1 1 3 0 1 0 2
```




```output7
2
1 1 100000 2 2 100000 1 2 2 1
```




```output8
0
5 4 4 3 4 4 4
```




```output9
1
1 1 1 1 1 1 1 1 0 1
```


