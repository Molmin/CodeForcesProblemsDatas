## Description

<div><p>Nikolay has <span class="tex-span"><i>a</i></span> lemons, <span class="tex-span"><i>b</i></span> apples and <span class="tex-span"><i>c</i></span> pears. He decided to cook a compote. According to the recipe the fruits should be in the ratio <span class="tex-span">1: 2: 4</span>. It means that for each lemon in the compote should be exactly <span class="tex-span">2</span> apples and exactly <span class="tex-span">4</span> pears. You can't crumble up, break up or cut these fruits into pieces. These fruits&nbsp;— lemons, apples and pears&nbsp;— should be put in the compote as whole fruits.</p><p>Your task is to determine the maximum total number of lemons, apples and pears from which Nikolay can cook the compote. It is possible that Nikolay can't use any fruits, in this case print <span class="tex-span">0</span>. </p></div><div class="input-specification"><p>The first line contains the positive integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 1000</span>)&nbsp;— the number of lemons Nikolay has. </p><p>The second line contains the positive integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ 1000</span>)&nbsp;— the number of apples Nikolay has. </p><p>The third line contains the positive integer <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>c</i> ≤ 1000</span>)&nbsp;— the number of pears Nikolay has.</p></div><div class="output-specification"><p>Print the maximum total number of lemons, apples and pears from which Nikolay can cook the compote.</p></div>

## Input

<p>The first line contains the positive integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 1000</span>)&nbsp;— the number of lemons Nikolay has. </p><p>The second line contains the positive integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ 1000</span>)&nbsp;— the number of apples Nikolay has. </p><p>The third line contains the positive integer <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>c</i> ≤ 1000</span>)&nbsp;— the number of pears Nikolay has.</p>

## Output

<p>Print the maximum total number of lemons, apples and pears from which Nikolay can cook the compote.</p>





```input1
2
5
7

```




```input2
4
7
13

```




```input3
2
3
2

```




```output1
7

```




```output2
21

```




```output3
0

```



## Note

<p>In the first example Nikolay can use <span class="tex-span">1</span> lemon, <span class="tex-span">2</span> apples and <span class="tex-span">4</span> pears, so the answer is <span class="tex-span">1 + 2 + 4 = 7</span>.</p><p>In the second example Nikolay can use <span class="tex-span">3</span> lemons, <span class="tex-span">6</span> apples and <span class="tex-span">12</span> pears, so the answer is <span class="tex-span">3 + 6 + 12 = 21</span>.</p><p>In the third example Nikolay don't have enough pears to cook any compote, so the answer is <span class="tex-span">0</span>. </p>
