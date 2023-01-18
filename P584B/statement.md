## Description

<div><p>Kolya loves putting gnomes at the circle table and giving them coins, and Tanya loves studying triplets of gnomes, sitting in the vertexes of an equilateral triangle.</p><p>More formally, there are <span class="tex-span">3<i>n</i></span> gnomes sitting in a circle. Each gnome can have from <span class="tex-span">1</span> to <span class="tex-span">3</span> coins. Let's number the places in the order they occur in the circle by numbers from <span class="tex-span">0</span> to <span class="tex-span">3<i>n</i> - 1</span>, let the gnome sitting on the <span class="tex-span"><i>i</i></span>-th place have <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> coins. If there is an integer <span class="tex-span"><i>i</i></span> (<span class="tex-span">0 ≤ <i>i</i> &lt; <i>n</i></span>) such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>i</i> + <i>n</i></sub> + <i>a</i><sub class="lower-index"><i>i</i> + 2<i>n</i></sub> ≠ 6</span>, then Tanya is satisfied. </p><p>Count the number of ways to choose <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> so that Tanya is satisfied. As there can be many ways of distributing coins, print the remainder of this number modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Two ways, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, are considered distinct if there is index <span class="tex-span"><i>i</i></span> (<span class="tex-span">0 ≤ <i>i</i> &lt; 3<i>n</i></span>), such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span> (that is, some gnome got different number of coins in these two ways).</p></div><div class="input-specification"><p>A single line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of the gnomes divided by three.</p></div><div class="output-specification"><p>Print a single number — the remainder of the number of variants of distributing coins that satisfy Tanya modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>A single line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of the gnomes divided by three.</p>

## Output

<p>Print a single number — the remainder of the number of variants of distributing coins that satisfy Tanya modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
1

```




```input2
2

```




```output1
20
```




```output2
680
```



## Note

<p><span class="tex-span">20</span> ways for <span class="tex-span"><i>n</i> = 1</span> (gnome with index <span class="tex-span">0</span> sits on the top of the triangle, gnome <span class="tex-span">1</span> on the right vertex, gnome <span class="tex-span">2</span> on the left vertex): <img class="tex-graphics" src="file://zz6HvNnr.png" style="max-width: 100.0%;max-height: 100.0%;"> </p><center> </center>
