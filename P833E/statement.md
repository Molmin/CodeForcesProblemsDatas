## Description

<div><center> <img class="tex-graphics" src="file://pu6LP4yQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It is well-known that the best decoration for a flower bed in Sweetland are vanilla muffins. Seedlings of this plant need sun to grow up. Slastyona has <span class="tex-span"><i>m</i></span> seedlings, and the <span class="tex-span"><i>j</i></span>-th seedling needs at least <span class="tex-span"><i>k</i><sub class="lower-index"><i>j</i></sub></span> minutes of sunlight to grow up.</p><p>Most of the time it's sunny in Sweetland, but sometimes some caramel clouds come, the <span class="tex-span"><i>i</i></span>-th of which will appear at time moment (minute) <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and disappear at time moment <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. Of course, the clouds make shadows, and the seedlings can't grow when there is at least one cloud veiling the sun.</p><p>Slastyona wants to grow up her muffins as fast as possible. She has exactly <span class="tex-span"><i>C</i></span> candies, which is the main currency in Sweetland. </p><p>One can dispel any cloud by paying <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> candies. However, in order to comply with Sweetland's Department of Meteorology regulations, <span class="tex-font-style-bf">one can't dispel more than two clouds</span>.</p><p>Slastyona hasn't decided yet which of the <span class="tex-span"><i>m</i></span> seedlings will be planted at the princess' garden, so she needs your help. For each seedling determine the earliest moment it can grow up if Slastyona won't break the law and won't spend more candies than she has. Note that each of the seedlings is considered independently.</p><p>The seedlings start to grow at time moment <span class="tex-span">0</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>C</i></span> <span class="tex-span">(0 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>, 0 ≤ <i>C</i> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;– the number of caramel clouds and the number of candies Slastyona has.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain three integers each: <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, describing one caramel cloud.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>&nbsp;– the number of seedlings. Each of the seedlings is described with one integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;– the required number of sunny minutes.</p></div><div class="output-specification"><p>For each seedling print one integer&nbsp;– the minimum minute Slastyona can grow it up.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>C</i></span> <span class="tex-span">(0 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>, 0 ≤ <i>C</i> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;– the number of caramel clouds and the number of candies Slastyona has.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain three integers each: <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, describing one caramel cloud.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>&nbsp;– the number of seedlings. Each of the seedlings is described with one integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;– the required number of sunny minutes.</p>

## Output

<p>For each seedling print one integer&nbsp;– the minimum minute Slastyona can grow it up.</p>





```input1
3 5
1 7 1
1 6 2
1 7 1
3
7
2
5

```




```input2
3 15
1 4 17
2 8 6
4 8 9
2
5
1

```




```input3
2 10
3 7 9
10 90 10
2
10
100

```




```output1
12
7
10

```




```output2
8
1

```




```output3
10
104

```



## Note

<p>Consider the first example. For each <span class="tex-span"><i>k</i></span> it is optimal to dispel clouds <span class="tex-span">1</span> and <span class="tex-span">3</span>. Then the remaining cloud will give shadow on time segment <span class="tex-span">[1..6]</span>. So, intervals <span class="tex-span">[0..1]</span> and <span class="tex-span">[6..<i>inf</i>)</span> are sunny.</p><center> <img class="tex-graphics" src="file://sqPfXUHb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example for <span class="tex-span"><i>k</i> = 1</span> it is not necessary to dispel anything, and for <span class="tex-span"><i>k</i> = 5</span> the best strategy is to dispel clouds <span class="tex-span">2</span> and <span class="tex-span">3</span>. This adds an additional sunny segment <span class="tex-span">[4..8]</span>, which together with <span class="tex-span">[0..1]</span> allows to grow up the muffin at the eight minute.</p><center> <img class="tex-graphics" src="file://f9L23kJL.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://WC4sqW15.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>If the third example the two seedlings are completely different. For the first one it is necessary to dispel cloud <span class="tex-span">1</span> and obtain a sunny segment <span class="tex-span">[0..10]</span>. However, the same strategy gives answer <span class="tex-span">180</span> for the second seedling. Instead, we can dispel cloud <span class="tex-span">2</span>, to make segments <span class="tex-span">[0..3]</span> and <span class="tex-span">[7..<i>inf</i>)</span> sunny, and this allows up to shorten the time to <span class="tex-span">104</span>.</p>
