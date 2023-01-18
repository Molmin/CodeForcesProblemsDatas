## Description

<div><p>Vasya plays the Geometry Horse.</p><p>The game goal is to destroy geometric figures of the game world. A certain number of points is given for destroying each figure depending on the figure type and the current factor value. </p><p>There are <span class="tex-span"><i>n</i></span> types of geometric figures. The number of figures of type <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and figure cost <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is known for each figure type. A player gets <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>·<i>f</i> </span> points for destroying one figure of type <span class="tex-span"><i>i</i></span>, where <span class="tex-span"><i>f</i></span> is the current factor. The factor value can be an integer number from <span class="tex-span">1</span> to <span class="tex-span"><i>t</i> + 1</span>, inclusive. At the beginning of the game the factor value is equal to 1. The factor is set to <span class="tex-span"><i>i</i> + 1</span> after destruction of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>t</i>)</span> figures, so the <span class="tex-span">(<i>p</i><sub class="lower-index"><i>i</i></sub> + 1)</span>-th figure to be destroyed is considered with factor equal to <span class="tex-span"><i>i</i> + 1</span>.</p><p>Your task is to determine the maximum number of points Vasya can get after he destroys all figures. Take into account that Vasya is so tough that he can destroy figures in any order chosen by him.</p></div><div class="input-specification"><p>The first line contains the only integer number <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of figure types.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integer numbers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>, separated with space — the number of figures of the <span class="tex-span"><i>i</i></span>-th type and the cost of one <span class="tex-span"><i>i</i></span>-type figure, correspondingly.</p><p>The next line contains the only integer number <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 100)</span> — the number that describe the factor's changes. </p><p>The next line contains <span class="tex-span"><i>t</i></span> integer numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>t</i></sub> ≤ 10<sup class="upper-index">12</sup>)</span>, separated with spaces.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div><div class="output-specification"><p>Print the only number — the maximum number of points Vasya can get.</p></div>

## Input

<p>The first line contains the only integer number <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of figure types.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integer numbers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>, separated with space — the number of figures of the <span class="tex-span"><i>i</i></span>-th type and the cost of one <span class="tex-span"><i>i</i></span>-type figure, correspondingly.</p><p>The next line contains the only integer number <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 100)</span> — the number that describe the factor's changes. </p><p>The next line contains <span class="tex-span"><i>t</i></span> integer numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>t</i></sub> ≤ 10<sup class="upper-index">12</sup>)</span>, separated with spaces.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>

## Output

<p>Print the only number — the maximum number of points Vasya can get.</p>





```input1
1
5 10
2
3 6

```




```input2
2
3 8
5 10
1
20

```




```output1
70
```




```output2
74
```



## Note

<p>In the first example Vasya destroys three figures first and gets <span class="tex-span">3·1·10 = 30</span> points. Then the factor will become equal to <span class="tex-span">2</span> and after destroying the last two figures Vasya will get <span class="tex-span">2·2·10 = 40</span> points. As a result Vasya will get <span class="tex-span">70</span> points.</p><p>In the second example all <span class="tex-span">8</span> figures will be destroyed with factor <span class="tex-span">1</span>, so Vasya will get <span class="tex-span">(3·8 + 5·10)·1 = 74</span> points.</p>
