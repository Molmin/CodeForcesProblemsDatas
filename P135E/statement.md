## Description

<div><p>Little Petya very much likes strings. Recently he has received a voucher to purchase a string as a gift from his mother. The string can be bought in the local shop. One can consider that the shop has all sorts of strings over the alphabet of fixed size. The size of the alphabet is equal to <span class="tex-span"><i>k</i></span>. However, the voucher has a string type limitation: specifically, the voucher can be used to purchase string <span class="tex-span"><i>s</i></span> if the length of string's longest substring that is also its weak subsequence (see the definition given below) equals <span class="tex-span"><i>w</i></span>.</p><p>String <span class="tex-span"><i>a</i></span> with the length of <span class="tex-span"><i>n</i></span> is considered the weak subsequence of the string <span class="tex-span"><i>s</i></span> with the length of <span class="tex-span"><i>m</i></span>, if there exists such a set of indexes <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>n</i></sub> ≤ <i>m</i></span>, that has the following two properties: </p><ul> <li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub> = <i>s</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub></span> for all <span class="tex-span"><i>k</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>; </li><li> there exists at least one such <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i></span>), for which <span class="tex-span"><i>i</i><sub class="lower-index"><i>k</i> + 1</sub> – <i>i</i><sub class="lower-index"><i>k</i></sub> &gt; 1</span>. </li></ul><p>Petya got interested how many different strings are available for him to purchase in the shop. As the number of strings can be very large, please find it modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). If there are infinitely many such strings, print "-1".</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>) and <span class="tex-span"><i>w</i></span> (<span class="tex-span">2 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>) — the alphabet size and the required length of the maximum substring that also is the weak subsequence, correspondingly.</p></div><div class="output-specification"><p>Print a single number — the number of strings Petya can buy using the voucher, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). If there are infinitely many such strings, print "-1" (without the quotes).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>) and <span class="tex-span"><i>w</i></span> (<span class="tex-span">2 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>) — the alphabet size and the required length of the maximum substring that also is the weak subsequence, correspondingly.</p>

## Output

<p>Print a single number — the number of strings Petya can buy using the voucher, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). If there are infinitely many such strings, print "-1" (without the quotes).</p>





```input1
2 2

```




```input2
3 5

```




```input3
2 139

```




```output1
10

```




```output2
1593

```




```output3
717248223

```



## Note

<p>In the first sample Petya can buy the following strings: aaa, aab, abab, abb, abba, baa, baab, baba, bba, bbb.</p>
