## Description

<div><p>Piglet has got a birthday today. His friend Winnie the Pooh wants to make the best present for him — a honey pot. Of course Winnie realizes that he won't manage to get the full pot to Piglet. In fact, he is likely to eat all the honey from the pot. And as soon as Winnie planned a snack on is way, the pot should initially have as much honey as possible. </p><p>The day before Winnie the Pooh replenished his honey stocks. Winnie-the-Pooh has <span class="tex-span"><i>n</i></span> shelves at home, each shelf contains some, perhaps zero number of honey pots. During the day Winnie came to the honey shelves <span class="tex-span"><i>q</i></span> times; on the <span class="tex-span"><i>i</i></span>-th time he came to some shelf <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, took from it some pots <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, tasted the honey from each pot and put all those pots on some shelf <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. As Winnie chose the pots, he followed his intuition. And that means that among all sets of <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> pots on shelf <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, he equiprobably chooses one.</p><p>Now Winnie remembers all actions he performed with the honey pots. He wants to take to the party the pot he didn't try the day before. For that he must know the mathematical expectation of the number <span class="tex-span"><i>m</i></span> of shelves that don't have a single <span class="tex-font-style-bf">untasted pot</span>. To evaluate his chances better, Winnie-the-Pooh wants to know the value <span class="tex-span"><i>m</i></span> after each action he performs.</p><p>Your task is to write a program that will find those values for him.</p></div><div class="input-specification"><p>The first line of the input contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of shelves at Winnie's place. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of honey pots on a shelf number <span class="tex-span"><i>i</i></span>. </p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of actions Winnie did the day before. Then follow <span class="tex-span"><i>q</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them describes an event that follows chronologically; the line contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 5</span>) — the number of the shelf from which Winnie took pots, the number of the shelf on which Winnie put the pots after he tasted each of them, and the number of the pots Winnie tasted, correspondingly.</p><p>Consider the shelves with pots numbered with integers from 1 to <span class="tex-span"><i>n</i></span>. It is guaranteed that Winnie-the-Pooh Never tried taking more pots from the shelf than it has.</p></div><div class="output-specification"><p>For each Winnie's action print the value of the mathematical expectation <span class="tex-span"><i>m</i></span> by the moment when this action is performed. The relative or absolute error of each value mustn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line of the input contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of shelves at Winnie's place. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of honey pots on a shelf number <span class="tex-span"><i>i</i></span>. </p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of actions Winnie did the day before. Then follow <span class="tex-span"><i>q</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them describes an event that follows chronologically; the line contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 5</span>) — the number of the shelf from which Winnie took pots, the number of the shelf on which Winnie put the pots after he tasted each of them, and the number of the pots Winnie tasted, correspondingly.</p><p>Consider the shelves with pots numbered with integers from 1 to <span class="tex-span"><i>n</i></span>. It is guaranteed that Winnie-the-Pooh Never tried taking more pots from the shelf than it has.</p>

## Output

<p>For each Winnie's action print the value of the mathematical expectation <span class="tex-span"><i>m</i></span> by the moment when this action is performed. The relative or absolute error of each value mustn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
3
2 2 3
5
1 2 1
2 1 2
1 2 2
3 1 1
3 2 2

```




```output1
0.000000000000
0.333333333333
1.000000000000
1.000000000000
2.000000000000

```


