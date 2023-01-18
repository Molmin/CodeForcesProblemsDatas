## Description

<div><p>Little Chris knows there's no fun in playing dominoes, he thinks it's too random and doesn't require skill. Instead, he decided to play <span class="tex-font-style-underline">with</span> the dominoes and make a "domino show".</p><p>Chris arranges <span class="tex-span"><i>n</i></span> dominoes in a line, placing each piece vertically upright. In the beginning, he simultaneously pushes some of the dominoes either to the left or to the right. However, somewhere between every two dominoes pushed in the same direction there is at least one domino pushed in the opposite direction.</p><p>After each second, each domino that is falling to the left pushes the adjacent domino on the left. Similarly, the dominoes falling to the right push their adjacent dominoes standing on the right. When a vertical domino has dominoes falling on it from both sides, it stays still due to the balance of the forces. The figure shows one possible example of the process.</p><center> <img class="tex-graphics" src="file://3fl9UyVV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Given the initial directions Chris has pushed the dominoes, find the number of the dominoes left standing vertically at the end of the process!</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>), the number of the dominoes in the line. The next line contains a character string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th character of the string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is equal to </p><ul> <li> "<span class="tex-font-style-tt">L</span>", if the <span class="tex-span"><i>i</i></span>-th domino has been pushed to the left; </li><li> "<span class="tex-font-style-tt">R</span>", if the <span class="tex-span"><i>i</i></span>-th domino has been pushed to the right; </li><li> "<span class="tex-font-style-tt">.</span>", if the <span class="tex-span"><i>i</i></span>-th domino has not been pushed. </li></ul><p>It is guaranteed that if <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>j</i></sub> = </span>"<span class="tex-font-style-tt">L</span>" and <span class="tex-span"><i>i</i> &lt; <i>j</i></span>, then there exists such <span class="tex-span"><i>k</i></span> that <span class="tex-span"><i>i</i> &lt; <i>k</i> &lt; <i>j</i></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub> = </span>"<span class="tex-font-style-tt">R</span>"; if <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>j</i></sub> = </span>"<span class="tex-font-style-tt">R</span>" and <span class="tex-span"><i>i</i> &lt; <i>j</i></span>, then there exists such <span class="tex-span"><i>k</i></span> that <span class="tex-span"><i>i</i> &lt; <i>k</i> &lt; <i>j</i></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub> = </span>"<span class="tex-font-style-tt">L</span>".</p></div><div class="output-specification"><p>Output a single integer, the number of the dominoes that remain vertical at the end of the process.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>), the number of the dominoes in the line. The next line contains a character string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th character of the string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is equal to </p><ul> <li> "<span class="tex-font-style-tt">L</span>", if the <span class="tex-span"><i>i</i></span>-th domino has been pushed to the left; </li><li> "<span class="tex-font-style-tt">R</span>", if the <span class="tex-span"><i>i</i></span>-th domino has been pushed to the right; </li><li> "<span class="tex-font-style-tt">.</span>", if the <span class="tex-span"><i>i</i></span>-th domino has not been pushed. </li></ul><p>It is guaranteed that if <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>j</i></sub> = </span>"<span class="tex-font-style-tt">L</span>" and <span class="tex-span"><i>i</i> &lt; <i>j</i></span>, then there exists such <span class="tex-span"><i>k</i></span> that <span class="tex-span"><i>i</i> &lt; <i>k</i> &lt; <i>j</i></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub> = </span>"<span class="tex-font-style-tt">R</span>"; if <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>j</i></sub> = </span>"<span class="tex-font-style-tt">R</span>" and <span class="tex-span"><i>i</i> &lt; <i>j</i></span>, then there exists such <span class="tex-span"><i>k</i></span> that <span class="tex-span"><i>i</i> &lt; <i>k</i> &lt; <i>j</i></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub> = </span>"<span class="tex-font-style-tt">L</span>".</p>

## Output

<p>Output a single integer, the number of the dominoes that remain vertical at the end of the process.</p>





```input1
14
.L.R...LR..L..

```




```input2
5
R....

```




```input3
1
.

```




```output1
4

```




```output2
0

```




```output3
1

```



## Note

<p>The first example case is shown on the figure. The four pieces that remain standing vertically are highlighted with orange.</p><p>In the second example case, all pieces fall down since the first piece topples all the other pieces.</p><p>In the last example case, a single piece has not been pushed in either direction.</p>
