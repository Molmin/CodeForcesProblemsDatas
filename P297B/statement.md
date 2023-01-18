## Description

<div><p>It is known that there are <span class="tex-span"><i>k</i></span> fish species in the polar ocean, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>. They are sorted by non-decreasing order of their weight, which is a positive number. Let the weight of the <span class="tex-span"><i>i</i></span>-th type of fish be <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, then <span class="tex-span">0 &lt; <i>w</i><sub class="lower-index">1</sub> ≤ <i>w</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>w</i><sub class="lower-index"><i>k</i></sub></span> holds.</p><p>Polar bears Alice and Bob each have caught some fish, and they are guessing who has the larger sum of weight of the fish he/she's caught. Given the type of the fish they've caught, determine whether it is possible that the fish caught by Alice has a <span class="tex-font-style-bf">strictly larger</span> total weight than Bob's. In other words, does there exist a sequence of weights <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (not necessary integers), such that the fish caught by Alice has a strictly larger total weight?</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the number of fish caught by Alice and Bob respectively, and the number of fish species.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers each from 1 to <span class="tex-span"><i>k</i></span>, the list of fish type caught by Alice. The third line contains <span class="tex-span"><i>m</i></span> integers each from 1 to <span class="tex-span"><i>k</i></span>, the list of fish type caught by Bob.</p><p>Note that one may have caught more than one fish for a same species.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the number of fish caught by Alice and Bob respectively, and the number of fish species.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers each from 1 to <span class="tex-span"><i>k</i></span>, the list of fish type caught by Alice. The third line contains <span class="tex-span"><i>m</i></span> integers each from 1 to <span class="tex-span"><i>k</i></span>, the list of fish type caught by Bob.</p><p>Note that one may have caught more than one fish for a same species.</p>

## Output

<p>Output "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p>





```input1
3 3 3
2 2 2
1 1 3

```




```input2
4 7 9
5 2 7 3
3 5 2 7 3 8 7

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample, if <span class="tex-span"><i>w</i><sub class="lower-index">1</sub> = 1, <i>w</i><sub class="lower-index">2</sub> = 2, <i>w</i><sub class="lower-index">3</sub> = 2.5</span>,  then Alice has a total of <span class="tex-span">2 + 2 + 2 = 6</span> weight units, while Bob only has <span class="tex-span">1 + 1 + 2.5 = 4.5</span>.</p><p>In the second sample, the fish that Alice caught is a subset of Bob's. Therefore, the total weight of Bob’s fish is always not less than the total weight of Alice’s fish.</p>
