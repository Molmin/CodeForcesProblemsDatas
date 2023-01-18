## Description

<div><p>Apart from plush toys, Imp is a huge fan of little yellow birds!</p><center> <img class="tex-graphics" src="file://Shy23D7O.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>To summon birds, Imp needs strong magic. There are <span class="tex-span"><i>n</i></span> trees in a row on an alley in a park, there is a nest on each of the trees. In the <span class="tex-span"><i>i</i></span>-th nest there are <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> birds; to summon one bird from this nest Imp needs to stay under this tree and it costs him <span class="tex-span"><i>cost</i><sub class="lower-index"><i>i</i></sub></span> points of mana. However, for each bird summoned, Imp increases his mana capacity by <span class="tex-span"><i>B</i></span> points. Imp summons birds one by one, he can summon any number from <span class="tex-span">0</span> to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> birds from the <span class="tex-span"><i>i</i></span>-th nest. </p><p>Initially Imp stands under the first tree and has <span class="tex-span"><i>W</i></span> points of mana, and his mana capacity equals <span class="tex-span"><i>W</i></span> as well. He can only go forward, and each time he moves from a tree to the next one, he restores <span class="tex-span"><i>X</i></span> points of mana (but it can't exceed his current mana capacity). Moving only forward, what is the maximum number of birds Imp can summon?</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>W</i></span>, <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>X</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>, 0 ≤ <i>W</i>, <i>B</i>, <i>X</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of trees, the initial points of mana, the number of points the mana capacity increases after a bird is summoned, and the number of points restored when Imp moves from a tree to the next one.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the number of birds living in the <span class="tex-span"><i>i</i></span>-th nest. It is guaranteed that <img align="middle" class="tex-formula" src="file://qkXrZBuj.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>cost</i><sub class="lower-index">1</sub>, <i>cost</i><sub class="lower-index">2</sub>, ..., <i>cost</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>cost</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>cost</i><sub class="lower-index"><i>i</i></sub></span> is the mana cost to summon a bird from the <span class="tex-span"><i>i</i></span>-th nest.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum number of birds Imp can summon.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>W</i></span>, <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>X</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>, 0 ≤ <i>W</i>, <i>B</i>, <i>X</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of trees, the initial points of mana, the number of points the mana capacity increases after a bird is summoned, and the number of points restored when Imp moves from a tree to the next one.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the number of birds living in the <span class="tex-span"><i>i</i></span>-th nest. It is guaranteed that <img align="middle" class="tex-formula" src="file://qkXrZBuj.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>cost</i><sub class="lower-index">1</sub>, <i>cost</i><sub class="lower-index">2</sub>, ..., <i>cost</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>cost</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>cost</i><sub class="lower-index"><i>i</i></sub></span> is the mana cost to summon a bird from the <span class="tex-span"><i>i</i></span>-th nest.</p>

## Output

<p>Print a single integer&nbsp;— the maximum number of birds Imp can summon.</p>





```input1
2 12 0 4
3 4
4 2

```




```input2
4 1000 10 35
1 2 4 5
1000 500 250 200

```




```input3
2 10 7 11
2 10
6 1

```




```output1
6

```




```output2
5

```




```output3
11

```



## Note

<p>In the first sample base amount of Imp's mana is equal to <span class="tex-span">12</span> (with maximum capacity also equal to <span class="tex-span">12</span>). After he summons two birds from the first nest, he loses <span class="tex-span">8</span> mana points, although his maximum capacity will not increase (since <span class="tex-span"><i>B</i> = 0</span>). After this step his mana will be <span class="tex-span">4</span> of <span class="tex-span">12</span>; during the move you will replenish <span class="tex-span">4</span> mana points, and hence own <span class="tex-span">8</span> mana out of <span class="tex-span">12</span> possible. Now it's optimal to take <span class="tex-span">4</span> birds from the second nest and spend <span class="tex-span">8</span> mana. The final answer will be — <span class="tex-span">6</span>.</p><p>In the second sample the base amount of mana is equal to <span class="tex-span">1000</span>. The right choice will be to simply pick all birds from the last nest. Note that Imp's mana doesn't restore while moving because it's initially full.</p>
