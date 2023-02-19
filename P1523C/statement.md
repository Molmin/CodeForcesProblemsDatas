## Description

<div><center> <img class="tex-graphics" height="378px" src="file://xSx7stEO.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>William is a huge fan of planning ahead. That is why he starts his morning routine by creating a nested list of upcoming errands.</p><p>A valid nested list is any list which can be created from a list with one item "<span class="tex-font-style-tt">1</span>" by applying some operations. Each operation inserts a new item into the list, <span class="tex-font-style-bf">on a new line</span>, just after one of existing items $a_1 \,.\, a_2 \,.\, a_3 \,.\, \,\cdots\, \,.\,a_k$ and can be one of two types: </p><ol> <li> Add an item $a_1 \,.\, a_2 \,.\, a_3 \,.\, \cdots \,.\, a_k \,.\, 1$ (starting a list of a deeper level), or </li><li> Add an item $a_1 \,.\, a_2 \,.\, a_3 \,.\, \cdots \,.\, (a_k + 1)$ (continuing the current level). </li></ol> Operation can only be applied if the list does not contain two identical items afterwards. And also, if we consider every item as a sequence of numbers, then the sequence of items should always remain increasing in lexicographical order. Examples of valid and invalid lists that are shown in the picture can found in the "<span class="tex-font-style-tt">Notes</span>" section.<p>When William decided to save a Word document with the list of his errands he accidentally hit a completely different keyboard shortcut from the "<span class="tex-font-style-tt">Ctrl-S</span>" he wanted to hit. It's not known exactly what shortcut he pressed but after triggering it all items in the list were replaced by a single number: the last number originally written in the item number.</p><p>William wants you to help him restore a fitting original nested list.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^3$), which is the number of lines in the list.</p><p>Each of the next $n$ lines contains a single integer $a_i$ ($1 \le a_i \le n$), which is what remains of William's nested list.</p><p>It is guaranteed that in each test case at least one fitting list exists.</p><p>It is guaranteed that the sum of values $n$ across all test cases does not exceed $10^3$.</p></div><div class="output-specification"><p>For each test case output $n$ lines which represent a valid nested list, which could become the data provided to you by William.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^3$), which is the number of lines in the list.</p><p>Each of the next $n$ lines contains a single integer $a_i$ ($1 \le a_i \le n$), which is what remains of William's nested list.</p><p>It is guaranteed that in each test case at least one fitting list exists.</p><p>It is guaranteed that the sum of values $n$ across all test cases does not exceed $10^3$.</p>

## Output

<p>For each test case output $n$ lines which represent a valid nested list, which could become the data provided to you by William.</p><p>If there are multiple answers, print any.</p>





```input1
2
4
1
1
2
3
9
1
1
1
2
2
1
2
1
2
```




```output1
1
1.1
1.2
1.3
1
1.1
1.1.1
1.1.2
1.2
1.2.1
2
2.1
2.2
```



## Note

<p>In the second example test case one example of a fitting list is:</p><p><span class="tex-font-style-bf">1</span></p><p>1.<span class="tex-font-style-bf">1</span> </p><p>1.1.<span class="tex-font-style-bf">1</span></p><p>1.1.<span class="tex-font-style-bf">2</span></p><p>1.<span class="tex-font-style-bf">2</span></p><p>1.2.<span class="tex-font-style-bf">1</span></p><p><span class="tex-font-style-bf">2</span></p><p>2.<span class="tex-font-style-bf">1</span></p><p>2.<span class="tex-font-style-bf">2</span></p><p>This list can be produced by using the sequence of operations shown below: <img class="tex-graphics" height="195px" src="file://D4mks9Lw.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </p><ol> <li> Original list with a single item $1$. </li><li> Insert item $2$ by using the insertion operation of the second type after item $1$. </li><li> Insert item $1.1$ by using the insertion operation of the first type after item $1$. </li><li> Insert item $1.2$ by using the insertion operation of the second type after item $1.1$. </li><li> Insert item $1.1.1$ by using the insertion operation of the first type after item $1.1$. </li><li> Insert item $1.1.2$ by using the insertion operation of the second type after item $1.1.1$. </li><li> Insert item $1.2.1$ by using the insertion operation of the first type after item $1.2$. </li><li> Insert item $2.1$ by using the insertion operation of the first type after item $2$. </li><li> Insert item $2.2$ by using the insertion operation of the second type after item $2.1$. </li></ol>
