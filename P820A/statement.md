## Description

<div><p>Mister B once received a gift: it was a book about aliens, which he started read immediately. This book had <span class="tex-span"><i>c</i></span> pages.</p><p>At first day Mister B read <span class="tex-span"><i>v</i><sub class="lower-index">0</sub></span> pages, but after that he started to speed up. Every day, starting from the second, he read <span class="tex-span"><i>a</i></span> pages more than on the previous day (at first day he read <span class="tex-span"><i>v</i><sub class="lower-index">0</sub></span> pages, at second&nbsp;— <span class="tex-span"><i>v</i><sub class="lower-index">0</sub> + <i>a</i></span> pages, at third&nbsp;— <span class="tex-span"><i>v</i><sub class="lower-index">0</sub> + 2<i>a</i></span> pages, and so on). But Mister B is just a human, so he physically wasn't able to read more than <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> pages per day.</p><p>Also, to refresh his memory, every day, starting from the second, Mister B had to reread last <span class="tex-span"><i>l</i></span> pages he read on the previous day. Mister B finished the book when he read the last page for the first time.</p><p>Help Mister B to calculate how many days he needed to finish the book.</p></div><div class="input-specification"><p>First and only line contains five space-separated integers: <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>c</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>l</i> &lt; <i>v</i><sub class="lower-index">0</sub> ≤ <i>v</i><sub class="lower-index">1</sub> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>a</i> ≤ 1000</span>) — the length of the book in pages, the initial reading speed, the maximum reading speed, the acceleration in reading speed and the number of pages for rereading.</p></div><div class="output-specification"><p>Print one integer — the number of days Mister B needed to finish the book.</p></div>

## Input

<p>First and only line contains five space-separated integers: <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>c</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>l</i> &lt; <i>v</i><sub class="lower-index">0</sub> ≤ <i>v</i><sub class="lower-index">1</sub> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>a</i> ≤ 1000</span>) — the length of the book in pages, the initial reading speed, the maximum reading speed, the acceleration in reading speed and the number of pages for rereading.</p>

## Output

<p>Print one integer — the number of days Mister B needed to finish the book.</p>





```input1
5 5 10 5 4

```




```input2
12 4 12 4 1

```




```input3
15 1 100 0 0

```




```output1
1

```




```output2
3

```




```output3
15

```



## Note

<p>In the first sample test the book contains <span class="tex-span">5</span> pages, so Mister B read it right at the first day.</p><p>In the second sample test at first day Mister B read pages number <span class="tex-span">1 - 4</span>, at second day&nbsp;— <span class="tex-span">4 - 11</span>, at third day&nbsp;— <span class="tex-span">11 - 12</span> and finished the book.</p><p>In third sample test every day Mister B read <span class="tex-span">1</span> page of the book, so he finished in 15 days.</p>
