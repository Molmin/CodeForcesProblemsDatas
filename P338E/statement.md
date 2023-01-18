## Description

<div><p>Manao is solving a problem with the following statement:</p><center> <img class="tex-graphics" src="file://FLDbptql.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>He came up with a solution that produces the correct answers but is too slow. You are given the pseudocode of his solution, where the function getAnswer calculates the answer to the problem:</p><pre class="verbatim"><br>getAnswer(a[1..n], b[1..len], h)<br>  answer = 0<br>  for i = 1 to n-len+1<br>    answer = answer + f(a[i..i+len-1], b, h, 1)<br>  return answer<br><br>f(s[1..len], b[1..len], h, index)<br>  if index = len+1 then<br>    return 1<br>  for i = 1 to len<br>    if s[index] + b[i] &gt;= h<br>      mem = b[i]<br>      b[i] = 0<br>      res = f(s, b, h, index + 1)<br>      b[i] = mem<br>      if res &gt; 0<br>        return 1<br>  return 0<br></pre><p>Your task is to help Manao optimize his algorithm.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>len</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>len</i> ≤ <i>n</i> ≤ 150000;&nbsp;1 ≤ <i>h</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains <span class="tex-span"><i>len</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>len</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print a single number — the answer to Manao's problem.</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>len</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>len</i> ≤ <i>n</i> ≤ 150000;&nbsp;1 ≤ <i>h</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains <span class="tex-span"><i>len</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>len</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print a single number — the answer to Manao's problem.</p>





```input1
5 2 10
5 3
1 8 5 5 7

```




```output1
2

```


