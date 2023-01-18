## Description

<div><p>You are given an image, that can be represented with a <span class="tex-span">2</span>-d <span class="tex-span"><i>n</i></span> by <span class="tex-span"><i>m</i></span> grid of pixels. Each pixel of the image is either on or off, denoted by the characters "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>", respectively. You would like to compress this image. You want to choose an integer <span class="tex-span"><i>k</i> &gt; 1</span> and split the image into <span class="tex-span"><i>k</i></span> by <span class="tex-span"><i>k</i></span> blocks. If <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> are not divisible by <span class="tex-span"><i>k</i></span>, the image is padded with only zeros on the right and bottom so that they are divisible by <span class="tex-span"><i>k</i></span>. Each pixel in each individual block must have the same value. The given image may not be compressible in its current state. Find the minimum number of pixels you need to toggle (after padding) in order for the image to be compressible for some <span class="tex-span"><i>k</i></span>. More specifically, the steps are to first choose <span class="tex-span"><i>k</i></span>, then the image is padded with zeros, then, we can toggle the pixels so it is compressible for this <span class="tex-span"><i>k</i></span>. The image must be compressible in that state.</p></div><div class="input-specification"><p>The first line of input will contain two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 2 500</span>), the dimensions of the image.</p><p>The next <span class="tex-span"><i>n</i></span> lines of input will contain a binary string with exactly <span class="tex-span"><i>m</i></span> characters, representing the image.</p></div><div class="output-specification"><p>Print a single integer, the minimum number of pixels needed to toggle to make the image compressible.</p></div>

## Input

<p>The first line of input will contain two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 2 500</span>), the dimensions of the image.</p><p>The next <span class="tex-span"><i>n</i></span> lines of input will contain a binary string with exactly <span class="tex-span"><i>m</i></span> characters, representing the image.</p>

## Output

<p>Print a single integer, the minimum number of pixels needed to toggle to make the image compressible.</p>





```input1
3 5
00100
10110
11001

```




```output1
5

```



## Note

<p>We first choose <span class="tex-span"><i>k</i> = 2</span>.</p><p>The image is padded as follows: </p><pre class="verbatim"><br>001000<br>101100<br>110010<br>000000<br></pre><p>We can toggle the image to look as follows: </p><pre class="verbatim"><br>001100<br>001100<br>000000<br>000000<br></pre><p>We can see that this image is compressible for <span class="tex-span"><i>k</i> = 2</span>.</p>
