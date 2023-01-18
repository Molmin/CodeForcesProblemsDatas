## Description

<div><p>Wilbur the pig really wants to be a beaver, so he decided today to pretend he is a beaver and bite at trees to cut them down.</p><p>There are <span class="tex-span"><i>n</i></span> trees located at various positions on a line. Tree <span class="tex-span"><i>i</i></span> is located at position <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. All the given positions of the trees are distinct.</p><p>The trees are equal, i.e. each tree has height <span class="tex-span"><i>h</i></span>. Due to the wind, when a tree is cut down, it either falls left with probability <span class="tex-span"><i>p</i></span>, or falls right with probability <span class="tex-span">1 - <i>p</i></span>. If a tree hits another tree while falling, that tree will fall in the same direction as the tree that hit it. A tree can hit another tree only if the distance between them is strictly less than <span class="tex-span"><i>h</i></span>. </p><p>For example, imagine there are <span class="tex-span">4</span> trees located at positions <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">5</span> and <span class="tex-span">8</span>, while <span class="tex-span"><i>h</i> = 3</span> and the tree at position <span class="tex-span">1</span> falls right. It hits the tree at position <span class="tex-span">3</span> and it starts to fall too. In it's turn it hits the tree at position <span class="tex-span">5</span> and it also starts to fall. The distance between <span class="tex-span">8</span> and <span class="tex-span">5</span> is exactly <span class="tex-span">3</span>, so the tree at position <span class="tex-span">8</span> will not fall.</p><p>As long as there are still trees standing, Wilbur will select either the leftmost standing tree with probability <span class="tex-span">0.5</span> or the rightmost standing tree with probability <span class="tex-span">0.5</span>. Selected tree is then cut down. If there is only one tree remaining, Wilbur always selects it. As the ground is covered with grass, Wilbur wants to know the expected total length of the ground covered with fallen trees after he cuts them all down because he is concerned about his grass-eating cow friends. Please help Wilbur.</p></div><div class="input-specification"><p>The first line of the input contains two integers, <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000)</span> and <span class="tex-span"><i>h</i></span> <span class="tex-span">(1 ≤ <i>h</i> ≤ 10<sup class="upper-index">8</sup>)</span> and a real number <span class="tex-span"><i>p</i></span> (<span class="tex-span">0 ≤ <i>p</i> ≤ 1</span>), given with no more than six decimal places.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span> in no particular order.</p></div><div class="output-specification"><p>Print a single real number&nbsp;— the expected total length of the ground covered by trees when they have all fallen down. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://2Vakh7l6.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains two integers, <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000)</span> and <span class="tex-span"><i>h</i></span> <span class="tex-span">(1 ≤ <i>h</i> ≤ 10<sup class="upper-index">8</sup>)</span> and a real number <span class="tex-span"><i>p</i></span> (<span class="tex-span">0 ≤ <i>p</i> ≤ 1</span>), given with no more than six decimal places.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span> in no particular order.</p>

## Output

<p>Print a single real number&nbsp;— the expected total length of the ground covered by trees when they have all fallen down. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://2Vakh7l6.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 2 0.500000
1 2

```




```input2
4 3 0.4
4 3 1 2

```




```output1
3.250000000

```




```output2
6.631200000

```



## Note

<p>Consider the first example, we have 2 trees with height 2. </p><center> <img class="tex-graphics" src="file://P22shMRu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> There are 3 scenarios: <p> 1. Both trees falls left. This can either happen with the right tree falling left first, which has <img align="middle" class="tex-formula" src="file://r7enMu64.png" style="max-width: 100.0%;max-height: 100.0%;"> probability (also knocking down the left tree), or the left tree can fall left and then the right tree can fall left, which has <img align="middle" class="tex-formula" src="file://9EC8Q9pB.png" style="max-width: 100.0%;max-height: 100.0%;"> probability. Total probability is <img align="middle" class="tex-formula" src="file://KnAy19tE.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p> 2. Both trees fall right. This is analogous to (1), so the probability of this happening is <img align="middle" class="tex-formula" src="file://1PiL8MIN.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p> 3. The left tree fall left and the right tree falls right. This is the only remaining scenario so it must have <img align="middle" class="tex-formula" src="file://eptNJmKU.png" style="max-width: 100.0%;max-height: 100.0%;"> probability. </p><p> Cases 1 and 2 lead to a total of 3 units of ground covered, while case 3 leads to a total of 4 units of ground covered. Thus, the expected value is <img align="middle" class="tex-formula" src="file://y872JKOH.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
