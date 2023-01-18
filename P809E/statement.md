## Description

<div><p>Tired of boring dates, Leha and Noora decided to play a game.</p><p>Leha found a tree with <span class="tex-span"><i>n</i></span> vertices numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. We remind you that tree is an undirected graph without cycles. Each vertex <span class="tex-span"><i>v</i></span> of a tree has a number <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i></sub></span> written on it. Quite by accident it turned out that all values written on vertices are distinct and are natural numbers between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>.</p><p>The game goes in the following way. Noora chooses some vertex <span class="tex-span"><i>u</i></span> of a tree uniformly at random and passes a move to Leha. Leha, in his turn, chooses (also uniformly at random) some vertex <span class="tex-span"><i>v</i></span> from remaining vertices of a tree <span class="tex-span">(<i>v</i> ≠ <i>u</i>)</span>. As you could guess there are <span class="tex-span"><i>n</i>(<i>n</i> - 1)</span> variants of choosing vertices by players. After that players calculate the value of a function <span class="tex-span"><i>f</i>(<i>u</i>, <i>v</i>) = φ(<i>a</i><sub class="lower-index"><i>u</i></sub>·<i>a</i><sub class="lower-index"><i>v</i></sub>)</span> <span class="tex-span">·</span> <span class="tex-span"><i>d</i>(<i>u</i>, <i>v</i>)</span> of the chosen vertices where <span class="tex-span">φ(<i>x</i>)</span> is Euler's totient function and <span class="tex-span"><i>d</i>(<i>x</i>, <i>y</i>)</span> is the shortest distance between vertices <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> in a tree.</p><p>Soon the game became boring for Noora, so Leha decided to defuse the situation and calculate expected value of function <span class="tex-span"><i>f</i></span> over all variants of choosing vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, hoping of at least somehow surprise the girl.</p><p>Leha asks for your help in calculating this expected value. Let this value be representable in the form of an irreducible fraction <img align="middle" class="tex-formula" src="file://C6EqlLfs.png" style="max-width: 100.0%;max-height: 100.0%;">. To further surprise Noora, he wants to name her the value <img align="middle" class="tex-formula" src="file://Tahz6w7F.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>Help Leha!</p></div><div class="input-specification"><p>The first line of input contains one integer number <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> &nbsp;— number of vertices in a tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> different numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> separated by spaces, denoting the values written on a tree vertices.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integer numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>)</span>, describing the next edge of a tree. It is guaranteed that this set of edges describes a tree.</p></div><div class="output-specification"><p>In a single line print a number equal to <span class="tex-span"><i>P</i>·<i>Q</i><sup class="upper-index"> - 1</sup></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input contains one integer number <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> &nbsp;— number of vertices in a tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> different numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> separated by spaces, denoting the values written on a tree vertices.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integer numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>)</span>, describing the next edge of a tree. It is guaranteed that this set of edges describes a tree.</p>

## Output

<p>In a single line print a number equal to <span class="tex-span"><i>P</i>·<i>Q</i><sup class="upper-index"> - 1</sup></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3
1 2 3
1 2
2 3

```




```input2
5
5 4 3 1 2
3 5
1 2
4 3
2 5

```




```output1
333333338

```




```output2
8

```



## Note

<p>Euler's totient function <span class="tex-span">φ(<i>n</i>)</span> is the number of such <span class="tex-span"><i>i</i></span> that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>,and <span class="tex-span"><i>gcd</i>(<i>i</i>, <i>n</i>) = 1</span>, where <span class="tex-span"><i>gcd</i>(<i>x</i>, <i>y</i>)</span> is the greatest common divisor of numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p><p>There are <span class="tex-span">6</span> variants of choosing vertices by Leha and Noora in the first testcase:</p><ul> <li> <span class="tex-span"><i>u</i> = 1</span>, <span class="tex-span"><i>v</i> = 2</span>, <span class="tex-span"><i>f</i>(1, 2) = φ(<i>a</i><sub class="lower-index">1</sub>·<i>a</i><sub class="lower-index">2</sub>)·<i>d</i>(1, 2) = φ(1·2)·1 = φ(2) = 1</span> </li><li> <span class="tex-span"><i>u</i> = 2</span>, <span class="tex-span"><i>v</i> = 1</span>, <span class="tex-span"><i>f</i>(2, 1) = <i>f</i>(1, 2) = 1</span> </li><li> <span class="tex-span"><i>u</i> = 1</span>, <span class="tex-span"><i>v</i> = 3</span>, <span class="tex-span"><i>f</i>(1, 3) = φ(<i>a</i><sub class="lower-index">1</sub>·<i>a</i><sub class="lower-index">3</sub>)·<i>d</i>(1, 3) = φ(1·3)·2 = 2φ(3) = 4</span> </li><li> <span class="tex-span"><i>u</i> = 3</span>, <span class="tex-span"><i>v</i> = 1</span>, <span class="tex-span"><i>f</i>(3, 1) = <i>f</i>(1, 3) = 4</span> </li><li> <span class="tex-span"><i>u</i> = 2</span>, <span class="tex-span"><i>v</i> = 3</span>, <span class="tex-span"><i>f</i>(2, 3) = φ(<i>a</i><sub class="lower-index">2</sub>·<i>a</i><sub class="lower-index">3</sub>)·<i>d</i>(2, 3) = φ(2·3)·1 = φ(6) = 2</span> </li><li> <span class="tex-span"><i>u</i> = 3</span>, <span class="tex-span"><i>v</i> = 2</span>, <span class="tex-span"><i>f</i>(3, 2) = <i>f</i>(2, 3) = 2</span> </li></ul><p>Expected value equals to <img align="middle" class="tex-formula" src="file://GOgS3Yq5.png" style="max-width: 100.0%;max-height: 100.0%;">. The value Leha wants to name Noora is <span class="tex-span">7·3<sup class="upper-index"> - 1</sup> = 7·333333336 = 333333338</span> <img align="middle" class="tex-formula" src="file://GXhoG2ub.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second testcase expected value equals to <img align="middle" class="tex-formula" src="file://NdjyHyMM.png" style="max-width: 100.0%;max-height: 100.0%;">, so Leha will have to surprise Hoora by number <span class="tex-span">8·1<sup class="upper-index"> - 1</sup> = 8</span> <img align="middle" class="tex-formula" src="file://Zgn5Eawc.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
