## Description

<div><p>You must have heard of the two brothers dreaming of ruling the world. With all their previous plans failed, this time they decided to cooperate with each other in order to rule the world. </p><p>As you know there are <span class="tex-span"><i>n</i></span> countries in the world. These countries are connected by <span class="tex-span"><i>n</i> - 1</span> directed roads. If you don't consider direction of the roads there is a unique path between every pair of countries in the world, passing through each road at most once. </p><p>Each of the brothers wants to establish his reign in some country, then it's possible for him to control the countries that can be reached from his country using directed roads. </p><p>The brothers can rule the world if there exists at most two countries for brothers to choose (and establish their reign in these countries) so that any other country is under control of at least one of them. In order to make this possible they want to change the direction of minimum number of roads. Your task is to calculate this minimum number of roads.</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3000)</span>. Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> saying there is a road from country <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to country <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Consider that countries are numbered from 1 to <span class="tex-span"><i>n</i></span>. It's guaranteed that if you don't consider direction of the roads there is a unique path between every pair of countries in the world, passing through each road at most once.</p></div><div class="output-specification"><p>In the only line of output print the minimum number of roads that their direction should be changed so that the brothers will be able to rule the world.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3000)</span>. Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> saying there is a road from country <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to country <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Consider that countries are numbered from 1 to <span class="tex-span"><i>n</i></span>. It's guaranteed that if you don't consider direction of the roads there is a unique path between every pair of countries in the world, passing through each road at most once.</p>

## Output

<p>In the only line of output print the minimum number of roads that their direction should be changed so that the brothers will be able to rule the world.</p>





```input1
4
2 1
3 1
4 1

```




```input2
5
2 1
2 3
4 3
4 5

```




```output1
1

```




```output2
0

```


