## Description

<div><p>Kirill plays a new computer game. He came to the potion store where he can buy any potion. Each potion is characterized by two integers&nbsp;— amount of experience and cost. The efficiency of a potion is the ratio of the amount of experience to the cost. Efficiency may be a non-integer number.</p><p>For each two integer numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> such that <span class="tex-span"><i>l</i> ≤ <i>a</i> ≤ <i>r</i></span> and <span class="tex-span"><i>x</i> ≤ <i>b</i> ≤ <i>y</i></span> there is a potion with experience <span class="tex-span"><i>a</i></span> and cost <span class="tex-span"><i>b</i></span> in the store (that is, there are <span class="tex-span">(<i>r</i> - <i>l</i> + 1)·(<i>y</i> - <i>x</i> + 1)</span> potions).</p><p>Kirill wants to buy a potion which has efficiency <span class="tex-span"><i>k</i></span>. Will he be able to do this?</p></div><div class="input-specification"><p>First string contains five integer numbers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">7</sup></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>y</i> ≤ 10<sup class="upper-index">7</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" without quotes if a potion with efficiency exactly <span class="tex-span"><i>k</i></span> can be bought in the store and "<span class="tex-font-style-tt">NO</span>" without quotes otherwise.</p><p>You can output each of the letters in any register.</p></div>

## Input

<p>First string contains five integer numbers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">7</sup></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>y</i> ≤ 10<sup class="upper-index">7</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" without quotes if a potion with efficiency exactly <span class="tex-span"><i>k</i></span> can be bought in the store and "<span class="tex-font-style-tt">NO</span>" without quotes otherwise.</p><p>You can output each of the letters in any register.</p>





```input1
1 10 1 10 1

```




```input2
1 5 6 10 1

```




```output1
YES
```




```output2
NO
```


