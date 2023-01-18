## Description

<div><p>Blake is the boss of Kris, however, this doesn't spoil their friendship. They often gather at the bar to talk about intriguing problems about maximising some values. This time the problem is really special.</p><p>You are given an array <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span>. The <span class="tex-font-style-it">characteristic</span> of this array is the value <img align="middle" class="tex-formula" src="file://aPVCD28q.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— the sum of the products of the values <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span"><i>i</i></span>. One may perform the following operation <span class="tex-font-style-bf">exactly once</span>: pick some element of the array and move to any position. In particular, it's allowed to move the element to the beginning or to the end of the array. Also, it's allowed to put it back to the initial position. The goal is to get the array with the maximum possible value of characteristic.</p><center> <img class="tex-graphics" src="file://AYgVyyM8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the size of the array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 1 000 000</span>)&nbsp;— the elements of the array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print a single integer — the maximum possible value of characteristic of <span class="tex-span"><i>a</i></span> that can be obtained by performing no more than one move.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the size of the array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 1 000 000</span>)&nbsp;— the elements of the array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print a single integer — the maximum possible value of characteristic of <span class="tex-span"><i>a</i></span> that can be obtained by performing no more than one move.</p>





```input1
4
4 3 2 5

```




```input2
5
1 1 2 7 1

```




```input3
3
1 1 2

```




```output1
39
```




```output2
49
```




```output3
9
```



## Note

<p>In the first sample, one may pick the first element and place it before the third (before <span class="tex-span">5</span>). Thus, the answer will be <span class="tex-span">3·1 + 2·2 + 4·3 + 5·4 = 39</span>.</p><p>In the second sample, one may pick the fifth element of the array and place it before the third. The answer will be <span class="tex-span">1·1 + 1·2 + 1·3 + 2·4 + 7·5 = 49</span>.</p>
