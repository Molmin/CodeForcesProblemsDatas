## Description

<div><p>In the pet store on sale there are:</p><ul> <li> $a$ packs of dog food; </li><li> $b$ packs of cat food; </li><li> $c$ packs of universal food (such food is suitable for both dogs and cats). </li></ul><p>Polycarp has $x$ dogs and $y$ cats. Is it possible that he will be able to buy food for all his animals in the store? Each of his dogs and each of his cats should receive one pack of suitable food for it.</p></div><div class="input-specification"><p>The first line of input contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the input.</p><p>Then $t$ lines are given, each containing a description of one test case. Each description consists of five integers $a, b, c, x$ and $y$ ($0 \le a,b,c,x,y \le 10^8$).</p></div><div class="output-specification"><p>For each test case in a separate line, output:</p><ul> <li> <span class="tex-font-style-tt">YES</span>, if suitable food can be bought for each of $x$ dogs and for each of $y$ cats; </li><li> <span class="tex-font-style-tt">NO</span> else. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p></div>

## Input

<p>The first line of input contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the input.</p><p>Then $t$ lines are given, each containing a description of one test case. Each description consists of five integers $a, b, c, x$ and $y$ ($0 \le a,b,c,x,y \le 10^8$).</p>

## Output

<p>For each test case in a separate line, output:</p><ul> <li> <span class="tex-font-style-tt">YES</span>, if suitable food can be bought for each of $x$ dogs and for each of $y$ cats; </li><li> <span class="tex-font-style-tt">NO</span> else. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p>





```input1
7
1 1 4 2 3
0 0 0 0 0
5 5 0 4 6
1 1 1 1 1
50000000 50000000 100000000 100000000 100000000
0 0 0 100000000 100000000
1 3 2 2 5
```




```output1
YES
YES
NO
YES
YES
NO
NO
```


