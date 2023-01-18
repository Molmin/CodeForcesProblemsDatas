## Description

<div><p>Flatland is inhabited by pixels of three colors: red, green and blue. We know that if two pixels of different colors meet in a violent fight, only one of them survives the fight (that is, the total number of pixels decreases by one). Besides, if pixels of colors <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(<i>x</i> ≠ <i>y</i>)</span> meet in a violent fight, then the pixel that survives the fight immediately changes its color to <span class="tex-span"><i>z</i></span> <span class="tex-span">(<i>z</i> ≠ <i>x</i>;&nbsp;<i>z</i> ≠ <i>y</i>)</span>. Pixels of the same color are friends, so they don't fight.</p><p>The King of Flatland knows that his land will be peaceful and prosperous when the pixels are of the same color. For each of the three colors you know the number of pixels of this color that inhabit Flatland. Help the king and determine whether fights can bring peace and prosperity to the country and if it is possible, find the minimum number of fights needed to make the land peaceful and prosperous. </p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> <span class="tex-span">(0 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 2<sup class="upper-index">31</sup>;&nbsp;<i>a</i> + <i>b</i> + <i>c</i> &gt; 0)</span> — the number of red, green and blue pixels, correspondingly.</p></div><div class="output-specification"><p>Print a single number — the minimum number of pixel fights before the country becomes peaceful and prosperous. If making the country peaceful and prosperous is impossible, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> <span class="tex-span">(0 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 2<sup class="upper-index">31</sup>;&nbsp;<i>a</i> + <i>b</i> + <i>c</i> &gt; 0)</span> — the number of red, green and blue pixels, correspondingly.</p>

## Output

<p>Print a single number — the minimum number of pixel fights before the country becomes peaceful and prosperous. If making the country peaceful and prosperous is impossible, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
1 1 1

```




```input2
3 1 0

```




```output1
1

```




```output2
3

```



## Note

<p>In the first test sample the country needs only one fight to achieve peace and prosperity. Besides, it can be any fight whatsoever. For example, let's assume that the green and the blue pixels fight, then the surviving pixel will be red. As a result, after the fight there are two red pixels. There won't be other pixels.</p><p>In the second sample the following sequence of fights is possible: red and blue, green and red, red and blue. As a result, after all fights there is one green pixel left.</p>
