## Description

<div><p>The night after the graduation ceremony graduate students of German University in Cairo (GUC) are playing darts. As there's no real dart board available, the photographs of members of the GUC upper management are being used.</p><p>So, <span class="tex-span"><i>n</i></span> rectangular photos are placed on the wall. They can overlap arbitrary and even coincide. The photos are not necessarily placed horizontally or vertically, they could also be rotated before being pinned to the wall.</p><p>The score of one dart throw is simply the number of photos the dart went through.</p><p>Fatma has made a throw but her score was not recorded. She only remembers that she did make it into at least one photo.</p><p>Assuming that the probability distribution of the throw is equal across the whole wall, what would be the expectation of Fatma's score?</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the number of photos on the wall. Then follow <span class="tex-span"><i>n</i></span> lines describing the photos, each containing <span class="tex-span">8</span> single-space-separated integers (coordinates of <span class="tex-span">4</span> vertices): <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">4</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">4</sub></span>. Each photo is a rectangle with a nonzero area. The coordinates are integers, not exceeding <span class="tex-span">10<sup class="upper-index">4</sup></span> by absolute value. The coordinates of the rectangle are given in either clockwise or counterclockwise order.</p></div><div class="output-specification"><p>Print the expected score of the throw. The answer will be accepted if it has absolute or relative error not exceeding <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the number of photos on the wall. Then follow <span class="tex-span"><i>n</i></span> lines describing the photos, each containing <span class="tex-span">8</span> single-space-separated integers (coordinates of <span class="tex-span">4</span> vertices): <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">4</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">4</sub></span>. Each photo is a rectangle with a nonzero area. The coordinates are integers, not exceeding <span class="tex-span">10<sup class="upper-index">4</sup></span> by absolute value. The coordinates of the rectangle are given in either clockwise or counterclockwise order.</p>

## Output

<p>Print the expected score of the throw. The answer will be accepted if it has absolute or relative error not exceeding <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
1
0 0 0 2 2 2 2 0

```




```input2
1
-1 0 0 1 1 0 0 -1

```




```input3
4
0 0 0 1 3 1 3 0
0 0 0 3 1 3 1 0
3 3 2 3 2 0 3 0
3 3 3 2 0 2 0 3

```




```input4
2
-1 0 0 1 1 0 0 -1
0 0 1 1 2 0 1 -1

```




```output1
1.0000000000

```




```output2
1.0000000000

```




```output3
1.5000000000

```




```output4
1.1428571429

```


