## Description

<div><p>One day Natalia was walking in the woods when she met a little mushroom gnome. The gnome told her the following story:</p><p>Everybody knows that the mushroom gnomes' power lies in the magic mushrooms that grow in the native woods of the gnomes. There are <span class="tex-span"><i>n</i></span> trees and <span class="tex-span"><i>m</i></span> magic mushrooms in the woods: the <span class="tex-span"><i>i</i></span>-th tree grows at a point on a straight line with coordinates <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and has the height of <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, the <span class="tex-span"><i>j</i></span>-th mushroom grows at the point with coordinates <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> and has magical powers <span class="tex-span"><i>z</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>But one day wild mushroommunchers, the sworn enemies of mushroom gnomes unleashed a terrible storm on their home forest. As a result, some of the trees began to fall and crush the magic mushrooms. The supreme oracle of mushroom gnomes calculated in advance the probability for each tree that it will fall to the left, to the right or will stand on. If the tree with the coordinate <span class="tex-span"><i>x</i></span> and height <span class="tex-span"><i>h</i></span> falls to the left, then all the mushrooms that belong to the right-open interval <span class="tex-span">[<i>x</i> - <i>h</i>, <i>x</i>)</span>, are destroyed. If a tree falls to the right, then the mushrooms that belong to the left-open interval <span class="tex-span">(<i>x</i>, <i>x</i> + <i>h</i>]</span> are destroyed. Only those mushrooms that are not hit by a single tree survive.</p><p>Knowing that all the trees fall independently of each other (i.e., all the events are mutually independent, and besides, the trees do not interfere with other trees falling in an arbitrary direction), the supreme oracle was also able to quickly calculate what would be the expectation of the total power of the mushrooms which survived after the storm. His calculations ultimately saved the mushroom gnomes from imminent death.</p><p>Natalia, as a good Olympiad programmer, got interested in this story, and she decided to come up with a way to quickly calculate the expectation of the sum of the surviving mushrooms' power.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of trees and mushrooms, respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contain four integers — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> + <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) which represent the coordinate of the <span class="tex-span"><i>i</i></span>-th tree, its height, the percentage of the probabilities that the tree falls to the left and to the right, respectively (the remaining percentage is the probability that the tree will stand on).</p><p>Each of next <span class="tex-span"><i>m</i></span> lines contain two integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">|<i>b</i><sub class="lower-index"><i>j</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>z</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">3</sup></span>) which represent the coordinate and the magical power of the <span class="tex-span"><i>j</i></span>-th mushroom, respectively.</p><p>An arbitrary number of trees and mushrooms can grow in one point.</p></div><div class="output-specification"><p>Print a real number — the expectation of the total magical power of the surviving mushrooms. The result is accepted with relative or absolute accuracy <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of trees and mushrooms, respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contain four integers — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> + <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) which represent the coordinate of the <span class="tex-span"><i>i</i></span>-th tree, its height, the percentage of the probabilities that the tree falls to the left and to the right, respectively (the remaining percentage is the probability that the tree will stand on).</p><p>Each of next <span class="tex-span"><i>m</i></span> lines contain two integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">|<i>b</i><sub class="lower-index"><i>j</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>z</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">3</sup></span>) which represent the coordinate and the magical power of the <span class="tex-span"><i>j</i></span>-th mushroom, respectively.</p><p>An arbitrary number of trees and mushrooms can grow in one point.</p>

## Output

<p>Print a real number — the expectation of the total magical power of the surviving mushrooms. The result is accepted with relative or absolute accuracy <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
1 1
2 2 50 50
1 1

```




```input2
2 1
2 2 50 50
4 2 50 50
3 1

```




```output1
0.5000000000

```




```output2
0.2500000000

```



## Note

<p>It is believed that the mushroom with the coordinate <span class="tex-span"><i>x</i></span> belongs to the right-open interval <span class="tex-span">[<i>l</i>, <i>r</i>)</span> if and only if <span class="tex-span"><i>l</i> ≤ <i>x</i> &lt; <i>r</i></span>. Similarly, the mushroom with the coordinate <span class="tex-span"><i>x</i></span> belongs to the left-open interval <span class="tex-span">(<i>l</i>, <i>r</i>]</span> if and only if <span class="tex-span"><i>l</i> &lt; <i>x</i> ≤ <i>r</i></span>.</p><p>In the first test the mushroom survives with the probability of 50%, depending on where the single tree falls.</p><p>In the second test the mushroom survives only if neither of the two trees falls on it. It occurs with the probability of 50% <span class="tex-span"> × </span> 50% = 25%.</p><p>Pretest №12 is the large test with <span class="tex-span">10<sup class="upper-index">5</sup></span> trees and one mushroom.</p>
