## Description

<div><p>In an attempt to make peace with the Mischievious Mess Makers, Bessie and Farmer John are planning to plant some flower gardens to complement the lush, grassy fields of Bovinia. As any good horticulturist knows, each garden they plant must have the exact same arrangement of flowers. Initially, Farmer John has <span class="tex-span"><i>n</i></span> different species of flowers he can plant, with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> flowers of the <span class="tex-span"><i>i</i></span>-th species.</p><p>On each of the next <span class="tex-span"><i>q</i></span> days, Farmer John will receive a batch of flowers of a new species. On day <span class="tex-span"><i>j</i></span>, he will receive <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> flowers of the same species, but of a different species from those Farmer John already has. </p><p>Farmer John, knowing the right balance between extravagance and minimalism, wants exactly <span class="tex-span"><i>k</i></span> species of flowers to be used. Furthermore, to reduce waste, each flower of the <span class="tex-span"><i>k</i></span> species Farmer John chooses must be planted in some garden. And each of the gardens must be identical; that is to say that each of the <span class="tex-span"><i>k</i></span> chosen species should have an equal number of flowers in each garden. As Farmer John is a proponent of national equality, he would like to create the greatest number of gardens possible.</p><p>After receiving flowers on each of these <span class="tex-span"><i>q</i></span> days, Farmer John would like to know the sum, over all possible choices of <span class="tex-span"><i>k</i></span> species, of the maximum number of gardens he could create. Since this could be a large number, you should output your result modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>).</p><p>The <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) of the next <span class="tex-span"><i>n</i></span> lines of the input contains an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>), the number of flowers of species <span class="tex-span"><i>i</i></span> Farmer John has initially.</p><p>The <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>q</i></span>) of the next <span class="tex-span"><i>q</i></span> lines of the input contains an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ 1 000 000</span>), the number of flowers of a new species Farmer John receives on day <span class="tex-span"><i>j</i></span>.</p></div><div class="output-specification"><p>After each of the <span class="tex-span"><i>q</i></span> days, output the sum of the maximum possible number of gardens, where the sum is taken over all possible choices of <span class="tex-span"><i>k</i></span> species, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>).</p><p>The <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) of the next <span class="tex-span"><i>n</i></span> lines of the input contains an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>), the number of flowers of species <span class="tex-span"><i>i</i></span> Farmer John has initially.</p><p>The <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>q</i></span>) of the next <span class="tex-span"><i>q</i></span> lines of the input contains an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ 1 000 000</span>), the number of flowers of a new species Farmer John receives on day <span class="tex-span"><i>j</i></span>.</p>

## Output

<p>After each of the <span class="tex-span"><i>q</i></span> days, output the sum of the maximum possible number of gardens, where the sum is taken over all possible choices of <span class="tex-span"><i>k</i></span> species, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 3 2
4
6
9
8
6

```




```input2
4 1 2
6
5
4
3
2
1

```




```output1
5
16

```




```output2
20
21

```



## Note

<p>In the first sample case, after the first day Farmer John has <span class="tex-span">(4, 6, 9, 8)</span> of each type of flower, and <span class="tex-span"><i>k</i> = 3</span>.</p><p>Choosing <span class="tex-span">(4, 6, 8)</span> lets him make <span class="tex-span">2</span> gardens, each with <span class="tex-span">(2, 3, 4)</span> of each flower, respectively. Choosing <span class="tex-span">(4, 6, 9)</span>, <span class="tex-span">(4, 9, 8)</span> and <span class="tex-span">(6, 9, 8)</span> each only let him make one garden, since there is no number of gardens that each species can be evenly split into. So the sum over all choices of <span class="tex-span"><i>k</i> = 3</span> flowers is <span class="tex-span">2 + 1 + 1 + 1 = 5</span>.</p><p>After the second day, Farmer John has <span class="tex-span">(4, 6, 9, 8, 6)</span> of each flower. The sum over all choices is <span class="tex-span">1 + 2 + 2 + 1 + 1 + 2 + 2 + 3 + 1 + 1 = 16</span>.</p><p>In the second sample case, <span class="tex-span"><i>k</i> = 1</span>. With <span class="tex-span"><i>x</i></span> flowers Farmer John can make <span class="tex-span"><i>x</i></span> gardens. So the answers to the queries are <span class="tex-span">6 + 5 + 4 + 3 + 2 = 20</span> and <span class="tex-span">6 + 5 + 4 + 3 + 2 + 1 = 21</span>.</p>
