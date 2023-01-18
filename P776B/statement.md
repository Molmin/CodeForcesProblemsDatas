## Description

<div><p>Sherlock has a new girlfriend (so unlike him!). Valentine's day is coming and he wants to gift her some jewelry.</p><p>He bought <span class="tex-span"><i>n</i></span> pieces of jewelry. The <span class="tex-span"><i>i</i></span>-th piece has price equal to <span class="tex-span"><i>i</i> + 1</span>, that is, the prices of the jewelry are <span class="tex-span">2, 3, 4, ... <i>n</i> + 1</span>.</p><p>Watson gave Sherlock a challenge to color these jewelry pieces such that two pieces don't have the same color if the price of one piece is a prime divisor of the price of the other piece. Also, Watson asked him to minimize the number of different colors used.</p><p>Help Sherlock complete this trivial task.</p></div><div class="input-specification"><p>The only line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>)&nbsp;— the number of jewelry pieces.</p></div><div class="output-specification"><p>The first line of output should contain a single integer <span class="tex-span"><i>k</i></span>, the minimum number of colors that can be used to color the pieces of jewelry with the given constraints.</p><p>The next line should consist of <span class="tex-span"><i>n</i></span> space-separated integers (between <span class="tex-span">1</span> and <span class="tex-span"><i>k</i></span>) that specify the color of each piece in the order of increasing price.</p><p>If there are multiple ways to color the pieces using <span class="tex-span"><i>k</i></span> colors, you can output any of them.</p></div>

## Input

<p>The only line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>)&nbsp;— the number of jewelry pieces.</p>

## Output

<p>The first line of output should contain a single integer <span class="tex-span"><i>k</i></span>, the minimum number of colors that can be used to color the pieces of jewelry with the given constraints.</p><p>The next line should consist of <span class="tex-span"><i>n</i></span> space-separated integers (between <span class="tex-span">1</span> and <span class="tex-span"><i>k</i></span>) that specify the color of each piece in the order of increasing price.</p><p>If there are multiple ways to color the pieces using <span class="tex-span"><i>k</i></span> colors, you can output any of them.</p>





```input1
3

```




```input2
4

```




```output1
2
1 1 2
```




```output2
2
2 1 1 2

```



## Note

<p>In the first input, the colors for first, second and third pieces of jewelry having respective prices <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span> are <span class="tex-span">1</span>, <span class="tex-span">1</span> and <span class="tex-span">2</span> respectively.</p><p>In this case, as <span class="tex-span">2</span> is a prime divisor of <span class="tex-span">4</span>, colors of jewelry having prices <span class="tex-span">2</span> and <span class="tex-span">4</span> must be distinct.</p>
