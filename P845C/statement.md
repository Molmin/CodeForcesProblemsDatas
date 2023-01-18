## Description

<div><p>Polycarp is a great fan of television.</p><p>He wrote down all the TV programs he is interested in for today. His list contains <span class="tex-span"><i>n</i></span> shows, <span class="tex-span"><i>i</i></span>-th of them starts at moment <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and ends at moment <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Polycarp owns two TVs. He can watch two different shows simultaneously with two TVs but he can only watch one show at any given moment on a single TV. If one show ends at the same moment some other show starts then you can't watch them on a single TV.</p><p>Polycarp wants to check out all <span class="tex-span"><i>n</i></span> shows. Are two TVs enough to do so?</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of shows.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — starting and ending time of <span class="tex-span"><i>i</i></span>-th show.</p></div><div class="output-specification"><p>If Polycarp is able to check out all the shows using only two TVs then print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of shows.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — starting and ending time of <span class="tex-span"><i>i</i></span>-th show.</p>

## Output

<p>If Polycarp is able to check out all the shows using only two TVs then print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
3
1 2
2 3
4 5

```




```input2
4
1 2
2 3
2 3
1 2

```




```output1
YES

```




```output2
NO

```


