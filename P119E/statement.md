## Description

<div><p>In the year of 3000 travelling around parallel realities became a routine thing. However one has to take into consideration that travelling like that is highly dangerous as you never know beforehand where you're gonna get...</p><p>Little Vasya, for instance, found himself in a gaming reality and now he has to successfully complete all levels of a very weird game to get back. The gaming reality is a three-dimensional space where <span class="tex-span"><i>n</i></span> points are given. The game has <span class="tex-span"><i>m</i></span> levels and at the beginning of the <span class="tex-span"><i>i</i></span>-th level the player is positioned at some plane <span class="tex-span"><i>Q</i><sub class="lower-index"><i>i</i></sub></span> that passes through the origin. On each level Vasya has to use special robots to construct and activate <span class="tex-span"><i>n</i></span> powerful energy spheres of the equal radius with centers at the given points. The player chooses the radius of the spheres himself. The player has to spend <span class="tex-span"><i>R</i></span> units of money to construct spheres whose radius equals <span class="tex-span"><i>R</i></span> (consequently, one can construct spheres whose radius equals zero for free). Besides, once for each level a player can choose any point in space and release a laser ray from there, perpendicular to plane <span class="tex-span"><i>Q</i><sub class="lower-index"><i>i</i></sub></span> (this action costs nothing). The ray can either be directed towards the plane or from the plane. The spheres that share at least one point with the ray will be immediately activated. The level is considered completed if the player has managed to activate all spheres. Note that the centers of the spheres are the same for all <span class="tex-span"><i>m</i></span> levels but the spheres do not remain: the player should construct them anew on each new level.</p><p>Help Vasya find out what minimum sum of money will be enough to complete each level.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 900, 1 ≤ <i>m</i> ≤ 100</span>) — the number of energetic spheres and the number of levels in the game correspondingly. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the coordinates of the center of the <span class="tex-span"><i>i</i></span>-th sphere. Assume that these points do not change their positions throughout the game.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines, each containing three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> + <i>b</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> + <i>c</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> &gt; 0</span>). These numbers are the coefficients in the equation of plane <span class="tex-span"><i>Q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><i>x</i> + <i>b</i><sub class="lower-index"><i>i</i></sub><i>y</i> + <i>c</i><sub class="lower-index"><i>i</i></sub><i>z</i> = 0</span>), where the player is positioned at the beginning of the <span class="tex-span"><i>i</i></span>-th level.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> numbers, one per line: the <span class="tex-span"><i>i</i></span>-th line should contain the minimum sum of money needed to complete the <span class="tex-span"><i>i</i></span>-th level. The absolute or relative error should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 900, 1 ≤ <i>m</i> ≤ 100</span>) — the number of energetic spheres and the number of levels in the game correspondingly. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the coordinates of the center of the <span class="tex-span"><i>i</i></span>-th sphere. Assume that these points do not change their positions throughout the game.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines, each containing three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> + <i>b</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> + <i>c</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> &gt; 0</span>). These numbers are the coefficients in the equation of plane <span class="tex-span"><i>Q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><i>x</i> + <i>b</i><sub class="lower-index"><i>i</i></sub><i>y</i> + <i>c</i><sub class="lower-index"><i>i</i></sub><i>z</i> = 0</span>), where the player is positioned at the beginning of the <span class="tex-span"><i>i</i></span>-th level.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> numbers, one per line: the <span class="tex-span"><i>i</i></span>-th line should contain the minimum sum of money needed to complete the <span class="tex-span"><i>i</i></span>-th level. The absolute or relative error should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
4 1
0 0 0
0 1 0
1 0 0
1 1 0
0 0 1

```




```input2
5 3
0 1 0
1 0 1
1 2 1
2 0 1
1 3 0
1 1 1
1 2 3
3 0 3

```




```input3
2 1
0 20 0
0 0 0
0 10 0

```




```output1
0.7071067812

```




```output2
1.6329931619
1.6366341768
1.5411035007

```




```output3
0.0000000000

```


