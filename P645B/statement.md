## Description

<div><p>It is a balmy spring afternoon, and Farmer John's <span class="tex-span"><i>n</i></span> cows are ruminating about link-cut cacti in their stalls. The cows, labeled <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>, are arranged so that the <span class="tex-span"><i>i</i></span>-th cow occupies the <span class="tex-span"><i>i</i></span>-th stall from the left. However, Elsie, after realizing that she will forever live in the shadows beyond Bessie's limelight, has formed the Mischievous Mess Makers and is plotting to disrupt this beautiful pastoral rhythm. While Farmer John takes his <span class="tex-span"><i>k</i></span> minute long nap, Elsie and the Mess Makers plan to repeatedly choose two distinct stalls and swap the cows occupying those stalls, making <span class="tex-font-style-bf">no more than one</span> swap each minute.</p><p>Being the meticulous pranksters that they are, the Mischievous Mess Makers would like to know the maximum messiness attainable in the <span class="tex-span"><i>k</i></span> minutes that they have. We denote as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> the label of the cow in the <span class="tex-span"><i>i</i></span>-th stall. The <span class="tex-font-style-it">messiness</span> of an arrangement of cows is defined as the number of pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> such that <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &gt; <i>p</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100 000</span>)&nbsp;— the number of cows and the length of Farmer John's nap, respectively.</p></div><div class="output-specification"><p>Output a single integer, the maximum messiness that the Mischievous Mess Makers can achieve by performing no more than <span class="tex-span"><i>k</i></span> swaps. </p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100 000</span>)&nbsp;— the number of cows and the length of Farmer John's nap, respectively.</p>

## Output

<p>Output a single integer, the maximum messiness that the Mischievous Mess Makers can achieve by performing no more than <span class="tex-span"><i>k</i></span> swaps. </p>





```input1
5 2

```




```input2
1 10

```




```output1
10

```




```output2
0

```



## Note

<p>In the first sample, the Mischievous Mess Makers can swap the cows in the stalls <span class="tex-span">1</span> and <span class="tex-span">5</span> during the first minute, then the cows in stalls <span class="tex-span">2</span> and <span class="tex-span">4</span> during the second minute. This reverses the arrangement of cows, giving us a total messiness of <span class="tex-span">10</span>.</p><p>In the second sample, there is only one cow, so the maximum possible messiness is <span class="tex-span">0</span>.</p>
