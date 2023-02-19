## Description

<div><p>Tarly has two different type of items, food boxes and wine barrels. There are <span class="tex-span"><i>f</i></span> food boxes and <span class="tex-span"><i>w</i></span> wine barrels. Tarly stores them in various stacks and each stack can consist of either food boxes or wine barrels but not both. The stacks are placed in a line such that no two stacks of food boxes are together and no two stacks of wine barrels are together.</p><p>The height of a stack is defined as the number of items in the stack. Two stacks are considered different if either their heights are different or one of them contains food and other contains wine.</p><p>Jon Snow doesn't like an arrangement if any stack of wine barrels has height less than or equal to <span class="tex-span"><i>h</i></span>. What is the probability that Jon Snow will like the arrangement if all arrangement are equiprobably?</p><p>Two arrangement of stacks are considered different if exists such <span class="tex-span"><i>i</i></span>, that <span class="tex-span"><i>i</i></span>-th stack of one arrangement is different from the <span class="tex-span"><i>i</i></span>-th stack of the other arrangement.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>f</i></span>, <span class="tex-span"><i>w</i></span>, <span class="tex-span"><i>h</i></span> (<span class="tex-span">0 ≤ <i>f</i>, <i>w</i>, <i>h</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of food boxes, number of wine barrels and <span class="tex-span"><i>h</i></span> is as described above. It is guaranteed that he has at least one food box or at least one wine barrel.</p></div><div class="output-specification"><p>Output the probability that Jon Snow will like the arrangement. The probability is of the form <img align="middle" class="tex-formula" src="file://zUhgwFBY.png" style="max-width: 100.0%;max-height: 100.0%;">, then you need to output a single integer <span class="tex-span"><i>p</i>·<i>q</i><sup class="upper-index"> - 1</sup> <i>mod</i> (10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>f</i></span>, <span class="tex-span"><i>w</i></span>, <span class="tex-span"><i>h</i></span> (<span class="tex-span">0 ≤ <i>f</i>, <i>w</i>, <i>h</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of food boxes, number of wine barrels and <span class="tex-span"><i>h</i></span> is as described above. It is guaranteed that he has at least one food box or at least one wine barrel.</p>

## Output

<p>Output the probability that Jon Snow will like the arrangement. The probability is of the form <img align="middle" class="tex-formula" src="file://zUhgwFBY.png" style="max-width: 100.0%;max-height: 100.0%;">, then you need to output a single integer <span class="tex-span"><i>p</i>·<i>q</i><sup class="upper-index"> - 1</sup> <i>mod</i> (10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1 1 1

```




```input2
1 2 1

```




```output1
0

```




```output2
666666672

```



## Note

<p>In the first example <span class="tex-span"><i>f</i>  =  1</span>, <span class="tex-span"><i>w</i> = 1</span> and <span class="tex-span"><i>h</i> = 1</span>, there are only two possible arrangement of stacks and Jon Snow doesn't like any of them.</p><p>In the second example <span class="tex-span"><i>f</i> = 1</span>, <span class="tex-span"><i>w</i> = 2</span> and <span class="tex-span"><i>h</i> = 1</span>, there are three arrangements. Jon Snow likes the (1) and (3) arrangement. So the probabilty is <img align="middle" class="tex-formula" src="file://tb5rQDZT.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><center> <img class="tex-graphics" src="file://28kcOX0z.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
