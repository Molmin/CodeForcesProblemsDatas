## Description

<div><p>It is lunch time for Mole. His friend, Marmot, prepared him a nice game for lunch.</p><p>Marmot brought Mole <span class="tex-span"><i>n</i></span> ordered piles of worms such that <span class="tex-span"><i>i</i></span>-th pile contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> worms. He labeled all these worms with consecutive integers: worms in first pile are labeled with numbers <span class="tex-span">1</span> to <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, worms in second pile are labeled with numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + 1</span> to <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub></span> and so on. See the example for a better understanding.</p><p>Mole can't eat all the worms (Marmot brought a lot) and, as we all know, Mole is blind, so Marmot tells him the labels of the best juicy worms. Marmot will only give Mole a worm if Mole says correctly in which pile this worm is contained.</p><p>Poor Mole asks for your help. For all juicy worms said by Marmot, tell Mole the correct answers.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of piles.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of worms in the <span class="tex-span"><i>i</i></span>-th pile.</p><p>The third line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of juicy worms said by Marmot.</p><p>The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub></span>), the labels of the juicy worms.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines to the standard output. The <span class="tex-span"><i>i</i></span>-th line should contain an integer, representing the number of the pile where the worm labeled with the number <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> is.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of piles.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of worms in the <span class="tex-span"><i>i</i></span>-th pile.</p><p>The third line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of juicy worms said by Marmot.</p><p>The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub></span>), the labels of the juicy worms.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines to the standard output. The <span class="tex-span"><i>i</i></span>-th line should contain an integer, representing the number of the pile where the worm labeled with the number <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> is.</p>





```input1
5
2 7 3 4 9
3
1 25 11

```




```output1
1
5
3

```



## Note

<p>For the sample input:</p><ul> <li> The worms with labels from [<span class="tex-span">1</span>, <span class="tex-span">2</span>] are in the first pile. </li><li> The worms with labels from [<span class="tex-span">3</span>, <span class="tex-span">9</span>] are in the second pile. </li><li> The worms with labels from [<span class="tex-span">10</span>, <span class="tex-span">12</span>] are in the third pile. </li><li> The worms with labels from [<span class="tex-span">13</span>, <span class="tex-span">16</span>] are in the fourth pile. </li><li> The worms with labels from [<span class="tex-span">17</span>, <span class="tex-span">25</span>] are in the fifth pile. </li></ul>
