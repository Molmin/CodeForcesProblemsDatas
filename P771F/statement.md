## Description

<div><p>Bearland is a big square on the plane. It contains all points with coordinates not exceeding <span class="tex-span">10<sup class="upper-index">6</sup></span> by the absolute value.</p><p>There are <span class="tex-span"><i>n</i></span> houses in Bearland. The <span class="tex-span"><i>i</i></span>-th of them is located at the point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. The <span class="tex-span"><i>n</i></span> points are distinct, but some subsets of them may be collinear.</p><p>Bear Limak lives in the first house. He wants to destroy his house and build a new one somewhere in Bearland.</p><p>Bears don't like big changes. For every three points (houses) <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>k</i></sub></span>, the sign of their cross product <span class="tex-span">(<i>p</i><sub class="lower-index"><i>j</i></sub> - <i>p</i><sub class="lower-index"><i>i</i></sub>) × (<i>p</i><sub class="lower-index"><i>k</i></sub> - <i>p</i><sub class="lower-index"><i>i</i></sub>)</span> should be the same before and after the relocation. If it was negative/positive/zero, it should still be negative/positive/zero respectively. This condition should be satisfied for all triples of indices <span class="tex-span">(<i>i</i>, <i>j</i>, <i>k</i>)</span>, possibly equal to each other or different than <span class="tex-span">1</span>. Additionally, Limak isn't allowed to build the house at the point where some other house already exists (but it can be the point where his old house was).</p><p>In the formula above, we define the difference and the cross product of points <span class="tex-span">(<i>a</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub>)</span> and <span class="tex-span">(<i>b</i><sub class="lower-index"><i>x</i></sub>, <i>b</i><sub class="lower-index"><i>y</i></sub>)</span> as: </p><center class="tex-equation"><span class="tex-span">(<i>a</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub>) - (<i>b</i><sub class="lower-index"><i>x</i></sub>, <i>b</i><sub class="lower-index"><i>y</i></sub>) = (<i>a</i><sub class="lower-index"><i>x</i></sub> - <i>b</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub> - <i>b</i><sub class="lower-index"><i>y</i></sub>), </span></center> <center class="tex-equation"><span class="tex-span">(<i>a</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub>) × (<i>b</i><sub class="lower-index"><i>x</i></sub>, <i>b</i><sub class="lower-index"><i>y</i></sub>) = <i>a</i><sub class="lower-index"><i>x</i></sub>·<i>b</i><sub class="lower-index"><i>y</i></sub> - <i>a</i><sub class="lower-index"><i>y</i></sub>·<i>b</i><sub class="lower-index"><i>x</i></sub>.</span></center><p>Consider a set of possible new placements of Limak's house. Your task is to find the area of that set of points.</p><p>Formally, let's say that Limak chooses the new placement randomly (each coordinate is chosen independently uniformly at random from the interval <span class="tex-span">[ - 10<sup class="upper-index">6</sup>, 10<sup class="upper-index">6</sup>]</span>). Let <span class="tex-span"><i>p</i></span> denote the probability of getting the allowed placement of new house. Let <span class="tex-span"><i>S</i></span> denote the area of Bearland (<span class="tex-span"><i>S</i> = 4·10<sup class="upper-index">12</sup></span>). Your task is to find <span class="tex-span"><i>p</i>·<i>S</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 500</span>)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of the description of a test case contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of houses.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— coordinates of the <span class="tex-span"><i>i</i></span>-th house. No two houses are located at the same point in the same test case. Limak lives in the first house.</p><p>The sum of <span class="tex-span"><i>n</i></span> won't exceed <span class="tex-span">200 000</span>.</p></div><div class="output-specification"><p>Print one real value, denoting the area of the set of points that are possible new placements of Limak's house.</p><p>Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. More precisely, let the jury's answer be <span class="tex-span"><i>b</i></span>, and your answer be <span class="tex-span"><i>a</i></span>. Then your answer will be accepted if and only if <img align="middle" class="tex-formula" src="file://yLEGIqEK.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 500</span>)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of the description of a test case contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of houses.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— coordinates of the <span class="tex-span"><i>i</i></span>-th house. No two houses are located at the same point in the same test case. Limak lives in the first house.</p><p>The sum of <span class="tex-span"><i>n</i></span> won't exceed <span class="tex-span">200 000</span>.</p>

## Output

<p>Print one real value, denoting the area of the set of points that are possible new placements of Limak's house.</p><p>Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. More precisely, let the jury's answer be <span class="tex-span"><i>b</i></span>, and your answer be <span class="tex-span"><i>a</i></span>. Then your answer will be accepted if and only if <img align="middle" class="tex-formula" src="file://yLEGIqEK.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4
4
5 3
0 1
10 1
3 51
3
-999123 700000
-950000 123456
-950000 987654
3
2 3
10 -1
-4 6
5
1 3
5 2
6 1
4 4
-3 3

```




```output1
250.000000000000
100000000000.000000000000
0.000000000000
6.562500000000

```



## Note

<p>In the sample test, there are <span class="tex-span">4</span> test cases.</p><p>In the first test case, there are four houses and Limak's one is in <span class="tex-span">(5, 3)</span>. The set of valid new placements form a triangle with vertices in points <span class="tex-span">(0, 1)</span>, <span class="tex-span">(10, 1)</span> and <span class="tex-span">(3, 51)</span>, without its sides. The area of such a triangle is <span class="tex-span">250</span>.</p><p>In the second test case, the set of valid new placements form a rectangle of width <span class="tex-span">50 000</span> and height <span class="tex-span">2 000 000</span>. Don't forget that the new placement must be inside the big square that represents Bearland.</p><p>In the third test case, the three given points are collinear. Each cross product is equal to <span class="tex-span">0</span> and it should be <span class="tex-span">0</span> after the relocation as well. Hence, Limak's new house must lie on the line that goes through the given points. Since it must also be inside the big square, new possible placements are limited to some segment (excluding the two points where the other houses are). The area of any segment is <span class="tex-span">0</span>.</p>
