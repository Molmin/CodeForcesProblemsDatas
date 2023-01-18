## Description

<div><p>Vasya plays The Elder Trolls IV: Oblivon. Oh, those creators of computer games! What they do not come up with! Absolutely unique monsters have been added to the The Elder Trolls IV: Oblivon. One of these monsters is Unkillable Slug. Why it is "Unkillable"? Firstly, because it can be killed with cutting weapon only, so lovers of two-handed amber hammers should find suitable knife themselves. Secondly, it is necessary to make so many cutting strokes to Unkillable Slug. Extremely many. Too many! </p><p>Vasya has already promoted his character to 80-th level and in order to gain level 81 he was asked to kill Unkillable Slug. The monster has a very interesting shape. It looks like a rectangular parallelepiped with size <span class="tex-span"><i>x</i> × <i>y</i> × <i>z</i></span>, consisting of undestructable cells <span class="tex-span">1 × 1 × 1</span>. At one stroke Vasya can cut the Slug along an imaginary grid, i.e. cut with a plane parallel to one of the parallelepiped side. Monster dies when amount of parts it is divided reaches some critical value.</p><p>All parts of monster do not fall after each cut, they remains exactly on its places. I. e. Vasya can cut several parts with one cut.</p><p>Vasya wants to know what the maximum number of pieces he can cut the Unkillable Slug into striking him at most <span class="tex-span"><i>k</i></span> times.</p><p>Vasya's character uses absolutely thin sword with infinite length.</p></div><div class="input-specification"><p>The first line of input contains four integer numbers <span class="tex-span"><i>x</i>, <i>y</i>, <i>z</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output the only number — the answer for the problem.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line of input contains four integer numbers <span class="tex-span"><i>x</i>, <i>y</i>, <i>z</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output the only number — the answer for the problem.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
2 2 2 3

```




```input2
2 2 2 1

```




```output1
8
```




```output2
2
```



## Note

<p>In the first sample Vasya make 3 pairwise perpendicular cuts. He cuts monster on two parts with the first cut, then he divides each part on two with the second cut, and finally he divides each of the 4 parts on two.</p>
