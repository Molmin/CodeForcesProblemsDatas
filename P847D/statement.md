## Description

<div><p>A new dog show on TV is starting next week. On the show dogs are required to demonstrate bottomless stomach, strategic thinking and self-preservation instinct. You and your dog are invited to compete with other participants and naturally you want to win!</p><p>On the show a dog needs to eat as many bowls of dog food as possible (bottomless stomach helps here). Dogs compete separately of each other and the rules are as follows:</p><p>At the start of the show the dog and the bowls are located on a line. The dog starts at position <span class="tex-span"><i>x</i> = 0</span> and <span class="tex-span"><i>n</i></span> bowls are located at positions <span class="tex-span"><i>x</i> = 1, <i>x</i> = 2, ..., <i>x</i> = <i>n</i></span>. The bowls are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. After the show starts the dog immediately begins to run to the right to the first bowl.</p><p>The food inside bowls is not ready for eating at the start because it is too hot (dog's self-preservation instinct prevents eating). More formally, the dog can eat from the <span class="tex-span"><i>i</i></span>-th bowl after <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> seconds from the start of the show or later.</p><p>It takes dog 1 second to move from the position <span class="tex-span"><i>x</i></span> to the position <span class="tex-span"><i>x</i> + 1</span>. The dog is not allowed to move to the left, the dog runs only to the right with the constant speed 1 distance unit per second. When the dog reaches a bowl (say, the bowl <span class="tex-span"><i>i</i></span>), the following cases are possible:</p><ul> <li> the food had cooled down (i.e. it passed at least <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> seconds from the show start): the dog immediately eats the food and runs to the right without any stop, </li><li> the food is hot (i.e. it passed less than <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> seconds from the show start): the dog has two options: to wait for the <span class="tex-span"><i>i</i></span>-th bowl, eat the food and continue to run at the moment <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> or to skip the <span class="tex-span"><i>i</i></span>-th bowl and continue to run to the right without any stop. </li></ul><p>After <span class="tex-span"><i>T</i></span> seconds from the start the show ends. If the dog reaches a bowl of food at moment <span class="tex-span"><i>T</i></span> the dog can not eat it. The show stops before <span class="tex-span"><i>T</i></span> seconds if the dog had run to the right of the last bowl.</p><p>You need to help your dog create a strategy with which the maximum possible number of bowls of food will be eaten in <span class="tex-span"><i>T</i></span> seconds.</p></div><div class="input-specification"><p>Two integer numbers are given in the first line - <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>T</i> ≤ 2·10<sup class="upper-index">9</sup></span>) — the number of bowls of food and the time when the dog is stopped.</p><p>On the next line numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) are given, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the moment of time when the <span class="tex-span"><i>i</i></span>-th bowl of food is ready for eating.</p></div><div class="output-specification"><p>Output a single integer — the maximum number of bowls of food the dog will be able to eat in <span class="tex-span"><i>T</i></span> seconds.</p></div>

## Input

<p>Two integer numbers are given in the first line - <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>T</i> ≤ 2·10<sup class="upper-index">9</sup></span>) — the number of bowls of food and the time when the dog is stopped.</p><p>On the next line numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) are given, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the moment of time when the <span class="tex-span"><i>i</i></span>-th bowl of food is ready for eating.</p>

## Output

<p>Output a single integer — the maximum number of bowls of food the dog will be able to eat in <span class="tex-span"><i>T</i></span> seconds.</p>





```input1
3 5
1 5 3

```




```input2
1 2
1

```




```input3
1 1
1

```




```output1
2

```




```output2
1

```




```output3
0

```



## Note

<p>In the first example the dog should skip the second bowl to eat from the two bowls (the first and the third).</p>
