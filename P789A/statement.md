## Description

<div><p>Anastasia loves going for a walk in Central Uzhlyandian Park. But she became uninterested in simple walking, so she began to collect Uzhlyandian pebbles. At first, she decided to collect all the pebbles she could find in the park.</p><p>She has only <span class="tex-font-style-bf">two pockets</span>. She can put at most <span class="tex-span"><i>k</i></span> pebbles in each pocket at the same time. There are <span class="tex-span"><i>n</i></span> different pebble types in the park, and there are <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> pebbles of the <span class="tex-span"><i>i</i></span>-th type. Anastasia is very responsible, so she never mixes pebbles of different types in same pocket. However, she can put different kinds of pebbles in different pockets at the same time. Unfortunately, she can't spend all her time collecting pebbles, so she can collect pebbles from the park only once a day.</p><p>Help her to find the minimum number of days needed to collect all the pebbles of Uzhlyandian Central Park, taking into consideration that Anastasia can't place pebbles of different types in same pocket.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of different pebble types and number of pebbles Anastasia can place in one pocket.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— number of pebbles of each type. </p></div><div class="output-specification"><p>The only line of output contains one integer&nbsp;— the minimum number of days Anastasia needs to collect all the pebbles.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of different pebble types and number of pebbles Anastasia can place in one pocket.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— number of pebbles of each type. </p>

## Output

<p>The only line of output contains one integer&nbsp;— the minimum number of days Anastasia needs to collect all the pebbles.</p>





```input1
3 2
2 3 4

```




```input2
5 4
3 1 8 9 7

```




```output1
3

```




```output2
5

```



## Note

<p>In the first sample case, Anastasia can collect all pebbles of the first type on the first day, of second type&nbsp;— on the second day, and of third type&nbsp;— on the third day.</p><p>Optimal sequence of actions in the second sample case: </p><ul> <li> In the first day Anastasia collects <span class="tex-span">8</span> pebbles of the third type. </li><li> In the second day she collects <span class="tex-span">8</span> pebbles of the fourth type. </li><li> In the third day she collects <span class="tex-span">3</span> pebbles of the first type and <span class="tex-span">1</span> pebble of the fourth type. </li><li> In the fourth day she collects <span class="tex-span">7</span> pebbles of the fifth type. </li><li> In the fifth day she collects <span class="tex-span">1</span> pebble of the second type. </li></ul>
