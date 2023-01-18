## Description

<div><p>Dima liked the present he got from Inna very much. He liked the present he got from Seryozha even more. </p><p>Dima felt so grateful to Inna about the present that he decided to buy her <span class="tex-span"><i>n</i></span> hares. Inna was very happy. She lined up the hares in a row, numbered them from 1 to <span class="tex-span"><i>n</i></span> from left to right and started feeding them with carrots. Inna was determined to feed each hare exactly once. But in what order should she feed them?</p><p>Inna noticed that each hare radiates joy when she feeds it. And the joy of the specific hare depends on whether Inna fed its adjacent hares before feeding it. Inna knows how much joy a hare radiates if it eats when either both of his adjacent hares are hungry, or one of the adjacent hares is full (that is, has been fed), or both of the adjacent hares are full. Please note that hares number 1 and <span class="tex-span"><i>n</i></span> don't have a left and a right-adjacent hare correspondingly, so they can never have two full adjacent hares.</p><p>Help Inna maximize the total joy the hares radiate. :)</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3000)</span> — the number of hares. Then three lines follow, each line has <span class="tex-span"><i>n</i></span> integers. The first line contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> <span class="tex-span">...</span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. The second line contains <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. The third line contains <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>. The following limits are fulfilled: <span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>.</p><p>Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> in the first line shows the joy that hare number <span class="tex-span"><i>i</i></span> gets if his adjacent hares are both hungry. Number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> in the second line shows the joy that hare number <span class="tex-span"><i>i</i></span> radiates if he has exactly one full adjacent hare. Number <span class="tex-span"><i>с</i><sub class="lower-index"><i>i</i></sub></span> in the third line shows the joy that hare number <span class="tex-span"><i>i</i></span> radiates if both his adjacent hares are full.</p></div><div class="output-specification"><p>In a single line, print the maximum possible total joy of the hares Inna can get by feeding them.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3000)</span> — the number of hares. Then three lines follow, each line has <span class="tex-span"><i>n</i></span> integers. The first line contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> <span class="tex-span">...</span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. The second line contains <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. The third line contains <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>. The following limits are fulfilled: <span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>.</p><p>Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> in the first line shows the joy that hare number <span class="tex-span"><i>i</i></span> gets if his adjacent hares are both hungry. Number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> in the second line shows the joy that hare number <span class="tex-span"><i>i</i></span> radiates if he has exactly one full adjacent hare. Number <span class="tex-span"><i>с</i><sub class="lower-index"><i>i</i></sub></span> in the third line shows the joy that hare number <span class="tex-span"><i>i</i></span> radiates if both his adjacent hares are full.</p>

## Output

<p>In a single line, print the maximum possible total joy of the hares Inna can get by feeding them.</p>





```input1
4
1 2 3 4
4 3 2 1
0 1 1 0

```




```input2
7
8 5 7 6 1 8 9
2 7 9 5 4 3 1
2 3 3 4 1 1 3

```




```input3
3
1 1 1
1 2 1
1 1 1

```




```output1
13

```




```output2
44

```




```output3
4

```


