## Description

<div><p>As Gerald ..., in other words, on a New Year Eve Constantine prepared an unusual present for the Beautiful Lady. The present is the magic New Year snowflake that can make any dream come true.</p><p>The New Year snowflake consists of tiny ice crystals, which can be approximately regarded as points on the plane. The beauty of the New Year snowflake is that it has a center of symmetry. This is a point such that for each crystal of the snowflake exists another crystal, symmetrical to it relative to that point. One of the crystals can be placed directly in the center of symmetry.</p><p>While Constantine was choosing a snowflake among millions of other snowflakes, no less symmetrical and no less magical, then endured a difficult path through the drifts to the house of his mistress, while he was waiting with bated breath for a few long moments before the Beautiful Lady opens the door, some of the snowflake crystals melted and naturally disappeared. Constantine is sure that there were no more than <span class="tex-span"><i>k</i></span> of such crystals, because he handled the snowflake very carefully. Now he is ready to demonstrate to the Beautiful Lady all the power of nanotechnology and restore the symmetry of snowflakes.</p><p>You are given the coordinates of the surviving snowflake crystals, given in nanometers. Your task is to identify all possible positions of the original center of symmetry.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10</span>) — the number of the surviving snowflake crystals and the maximum number of melted crystals, correspondingly. Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the crystals that are left in the following form: "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>". The coordinates are integers and do not exceed <span class="tex-span">5·10<sup class="upper-index">8</sup></span> in absolute value. All given points are different.</p></div><div class="output-specification"><p>The first line contains an integer <span class="tex-span"><i>c</i></span> — the number of possible symmetry centers. Next <span class="tex-span"><i>c</i></span> lines should contain the centers' descriptions. Each symmetry center is described by a couple of coordinates "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>", separated by a space. Print the coordinates with absolute error not exceeding <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. You are allowed to print the symmetry centers in any order. All printed points should be different. If there exist an infinite number of possible symmetry centers, print the single number "-1".</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10</span>) — the number of the surviving snowflake crystals and the maximum number of melted crystals, correspondingly. Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the crystals that are left in the following form: "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>". The coordinates are integers and do not exceed <span class="tex-span">5·10<sup class="upper-index">8</sup></span> in absolute value. All given points are different.</p>

## Output

<p>The first line contains an integer <span class="tex-span"><i>c</i></span> — the number of possible symmetry centers. Next <span class="tex-span"><i>c</i></span> lines should contain the centers' descriptions. Each symmetry center is described by a couple of coordinates "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>", separated by a space. Print the coordinates with absolute error not exceeding <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. You are allowed to print the symmetry centers in any order. All printed points should be different. If there exist an infinite number of possible symmetry centers, print the single number "-1".</p>





```input1
4 0
0 0
0 1
1 0
1 1

```




```input2
4 2
0 0
0 1
1 0
1 1

```




```input3
4 4
0 0
0 1
1 0
1 1

```




```output1
1
0.5 0.5

```




```output2
5
0.0 0.5
0.5 0.0
0.5 0.5
0.5 1.0
1.0 0.5

```




```output3
-1

```


