## Description

<div><p>Mole is hungry again. He found one ant colony, consisting of <span class="tex-span"><i>n</i></span> ants, ordered in a row. Each ant <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) has a strength <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>In order to make his dinner more interesting, Mole organizes a version of «Hunger Games» for the ants. He chooses two numbers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) and each pair of ants with indices between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (inclusively) will fight. When two ants <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> fight, ant <span class="tex-span"><i>i</i></span> gets one battle point only if <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> divides <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub></span> (also, ant <span class="tex-span"><i>j</i></span> gets one battle point only if <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub></span> divides <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>). </p><p>After all fights have been finished, Mole makes the ranking. An ant <span class="tex-span"><i>i</i></span>, with <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> battle points obtained, is going to be freed only if <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> = <i>r</i> - <i>l</i></span>, or in other words only if it took a point in every fight it participated. After that, Mole eats the rest of the ants. Note that there can be many ants freed or even none.</p><p>In order to choose the best sequence, Mole gives you <span class="tex-span"><i>t</i></span> segments <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> and asks for each of them how many ants is he going to eat if those ants fight.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the size of the ant colony. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the strengths of the ants. </p><p>The third line contains one integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of test cases. </p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), describing one query.</p></div><div class="output-specification"><p>Print to the standard output <span class="tex-span"><i>t</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line contains number of ants that Mole eats from the segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the size of the ant colony. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the strengths of the ants. </p><p>The third line contains one integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of test cases. </p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), describing one query.</p>

## Output

<p>Print to the standard output <span class="tex-span"><i>t</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line contains number of ants that Mole eats from the segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p>





```input1
5
1 3 2 4 2
4
1 5
2 5
3 5
4 5

```




```output1
4
4
1
1

```



## Note

<p>In the first test battle points for each ant are <span class="tex-span"><i>v</i> = [4, 0, 2, 0, 2]</span>, so ant number <span class="tex-span">1</span> is freed. Mole eats the ants <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">5</span>.</p><p>In the second test case battle points are <span class="tex-span"><i>v</i> = [0, 2, 0, 2]</span>, so no ant is freed and all of them are eaten by Mole.</p><p>In the third test case battle points are <span class="tex-span"><i>v</i> = [2, 0, 2]</span>, so ants number <span class="tex-span">3</span> and <span class="tex-span">5</span> are freed. Mole eats <span class="tex-font-style-bf">only the ant <span class="tex-span">4</span></span>.</p><p>In the fourth test case battle points are <span class="tex-span"><i>v</i> = [0, 1]</span>, so ant number <span class="tex-span">5</span> is freed. Mole eats the ant <span class="tex-span">4</span>.</p>
