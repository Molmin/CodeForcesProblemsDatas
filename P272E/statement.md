## Description

<div><p>Dima came to the horse land. There are <span class="tex-span"><i>n</i></span> horses living in the land. Each horse in the horse land has several enemies (enmity is a symmetric relationship). The horse land isn't very hostile, so the number of enemies of each horse is at most 3.</p><p>Right now the horse land is going through an election campaign. So the horses trusted Dima to split them into two parts. At that the horses want the following condition to hold: a horse shouldn't have more than one enemy in its party.</p><p>Help Dima split the horses into parties. Note that one of the parties can turn out to be empty.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <img align="middle" class="tex-formula" src="file://9K9sILyI.png" style="max-width: 100.0%;max-height: 100.0%;"> — the number of horses in the horse land and the number of enemy pairs.</p><p>Next <span class="tex-span"><i>m</i></span> lines define the enemy pairs. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, which mean that horse <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the enemy of horse <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Consider the horses indexed in some way from 1 to <span class="tex-span"><i>n</i></span>. It is guaranteed that each horse has at most three enemies. No pair of enemies occurs more than once in the input.</p></div><div class="output-specification"><p>Print a line, consisting of <span class="tex-span"><i>n</i></span> characters: the <span class="tex-span"><i>i</i></span>-th character of the line must equal "<span class="tex-font-style-tt">0</span>", if the horse number <span class="tex-span"><i>i</i></span> needs to go to the first party, otherwise this character should equal "<span class="tex-font-style-tt">1</span>".</p><p>If there isn't a way to divide the horses as required, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <img align="middle" class="tex-formula" src="file://9K9sILyI.png" style="max-width: 100.0%;max-height: 100.0%;"> — the number of horses in the horse land and the number of enemy pairs.</p><p>Next <span class="tex-span"><i>m</i></span> lines define the enemy pairs. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, which mean that horse <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the enemy of horse <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Consider the horses indexed in some way from 1 to <span class="tex-span"><i>n</i></span>. It is guaranteed that each horse has at most three enemies. No pair of enemies occurs more than once in the input.</p>

## Output

<p>Print a line, consisting of <span class="tex-span"><i>n</i></span> characters: the <span class="tex-span"><i>i</i></span>-th character of the line must equal "<span class="tex-font-style-tt">0</span>", if the horse number <span class="tex-span"><i>i</i></span> needs to go to the first party, otherwise this character should equal "<span class="tex-font-style-tt">1</span>".</p><p>If there isn't a way to divide the horses as required, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
3 3
1 2
3 2
3 1

```




```input2
2 1
2 1

```




```input3
10 6
1 2
1 3
1 4
2 3
2 4
3 4

```




```output1
100

```




```output2
00

```




```output3
0110000000

```


