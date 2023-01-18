## Description

<div><p>All cities of Lineland are located on the <span class="tex-span"><i>Ox</i></span> coordinate axis. Thus, each city is associated with its position <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> — a coordinate on the <span class="tex-span"><i>Ox</i></span> axis. No two cities are located at a single point.</p><p>Lineland residents love to send letters to each other. A person may send a letter only if the recipient lives in another city (because if they live in the same city, then it is easier to drop in).</p><p>Strange but true, the cost of sending the letter is exactly equal to the distance between the sender's city and the recipient's city.</p><p>For each city calculate two values ​​<span class="tex-span"><i>min</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>max</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>min</i><sub class="lower-index"><i>i</i></sub></span> is the minimum cost of sending a letter from the <span class="tex-span"><i>i</i></span>-th city to some other city, and <span class="tex-span"><i>max</i><sub class="lower-index"><i>i</i></sub></span> is the the maximum cost of sending a letter from the <span class="tex-span"><i>i</i></span>-th city to some other city</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities in Lineland. The second line contains the sequence of <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>x</i></span>-coordinate of the <span class="tex-span"><i>i</i></span>-th city. All the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>'s are distinct and follow in <span class="tex-font-style-bf">ascending</span> order.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line must contain two integers <span class="tex-span"><i>min</i><sub class="lower-index"><i>i</i></sub>, <i>max</i><sub class="lower-index"><i>i</i></sub></span>, separated by a space, where <span class="tex-span"><i>min</i><sub class="lower-index"><i>i</i></sub></span> is the minimum cost of sending a letter from the <span class="tex-span"><i>i</i></span>-th city, and <span class="tex-span"><i>max</i><sub class="lower-index"><i>i</i></sub></span> is the maximum cost of sending a letter from the <span class="tex-span"><i>i</i></span>-th city.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities in Lineland. The second line contains the sequence of <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>x</i></span>-coordinate of the <span class="tex-span"><i>i</i></span>-th city. All the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>'s are distinct and follow in <span class="tex-font-style-bf">ascending</span> order.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line must contain two integers <span class="tex-span"><i>min</i><sub class="lower-index"><i>i</i></sub>, <i>max</i><sub class="lower-index"><i>i</i></sub></span>, separated by a space, where <span class="tex-span"><i>min</i><sub class="lower-index"><i>i</i></sub></span> is the minimum cost of sending a letter from the <span class="tex-span"><i>i</i></span>-th city, and <span class="tex-span"><i>max</i><sub class="lower-index"><i>i</i></sub></span> is the maximum cost of sending a letter from the <span class="tex-span"><i>i</i></span>-th city.</p>





```input1
4
-5 -2 2 7

```




```input2
2
-1 1

```




```output1
3 12
3 9
4 7
5 12

```




```output2
2 2
2 2

```


