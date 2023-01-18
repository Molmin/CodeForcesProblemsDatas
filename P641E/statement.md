## Description

<div><p>Little Artem has invented a time machine! He could go anywhere in time, but all his thoughts of course are with computer science. He wants to apply this time machine to a well-known data structure: <span class="tex-font-style-underline">multiset</span>.</p><p>Artem wants to create a basic multiset of integers. He wants these structure to support operations of three types:</p><ol> <li> Add integer to the multiset. Note that the difference between set and multiset is that multiset may store several instances of one integer. </li><li> Remove integer from the multiset. Only one instance of this integer is removed. Artem doesn't want to handle any exceptions, so he assumes that every time remove operation is called, that integer is presented in the multiset. </li><li> Count the number of instances of the given integer that are stored in the multiset. </li></ol><p>But what about time machine? Artem doesn't simply apply operations to the multiset one by one, he now travels to different moments of time and apply his operation there. Consider the following example.</p><ul> <li> First Artem adds integer <span class="tex-span">5</span> to the multiset at the <span class="tex-span">1</span>-st moment of time. </li><li> Then Artem adds integer <span class="tex-span">3</span> to the multiset at the moment <span class="tex-span">5</span>. </li><li> Then Artem asks how many <span class="tex-span">5</span> are there in the multiset at moment <span class="tex-span">6</span>. The answer is <span class="tex-span">1</span>. </li><li> Then Artem returns back in time and asks how many integers <span class="tex-span">3</span> are there in the set at moment <span class="tex-span">4</span>. Since <span class="tex-span">3</span> was added only at moment <span class="tex-span">5</span>, the number of integers <span class="tex-span">3</span> at moment <span class="tex-span">4</span> equals to <span class="tex-span">0</span>. </li><li> Then Artem goes back in time again and removes <span class="tex-span">5</span> from the multiset at moment <span class="tex-span">3</span>. </li><li> Finally Artyom asks at moment <span class="tex-span">7</span> how many integers <span class="tex-span">5</span> are there in the set. The result is <span class="tex-span">0</span>, since we have removed <span class="tex-span">5</span> at the moment <span class="tex-span">3</span>. </li></ul><p>Note that Artem dislikes exceptions so much that he assures that after each change he makes all delete operations are applied only to element that is present in the multiset. The answer to the query of the third type is computed at the moment Artem makes the corresponding query and are not affected in any way by future changes he makes.</p><p>Help Artem implement time travellers multiset.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of Artem's queries.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines with queries descriptions. Each of them contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— type of the query, moment of time Artem travels to in order to execute this query and the value of the query itself, respectively. It's guaranteed that all moments of time are distinct and that after each operation is applied all operations of the first and second types are consistent.</p></div><div class="output-specification"><p>For each ask operation output the number of instances of integer being queried at the given moment of time.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of Artem's queries.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines with queries descriptions. Each of them contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— type of the query, moment of time Artem travels to in order to execute this query and the value of the query itself, respectively. It's guaranteed that all moments of time are distinct and that after each operation is applied all operations of the first and second types are consistent.</p>

## Output

<p>For each ask operation output the number of instances of integer being queried at the given moment of time.</p>





```input1
6
1 1 5
3 5 5
1 2 5
3 6 5
2 3 5
3 7 5

```




```input2
3
1 1 1
2 2 1
3 3 1

```




```output1
1
2
1

```




```output2
0

```


