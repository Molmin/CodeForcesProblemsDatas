## Description

<div><p>Arkady and Kirill visited an exhibition of rare coins. The coins were located in a row and enumerated from left to right from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>, each coin either was laid with its obverse (front) side up, or with its reverse (back) side up.</p><p>Arkady and Kirill made some photos of the coins, each photo contained a segment of neighboring coins. Akrady is interested in obverses, so on each photo made by him there is at least one coin with obverse side up. On the contrary, Kirill is interested in reverses, so on each photo made by him there is at least one coin with its reverse side up.</p><p>The photos are lost now, but Arkady and Kirill still remember the bounds of the segments of coins each photo contained. Given this information, compute the remainder of division by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> of the number of ways to choose the upper side of each coin in such a way, that on each Arkady's photo there is at least one coin with obverse side up, and on each Kirill's photo there is at least one coin with reverse side up.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the total number of coins, the number of photos made by Arkady, and the number of photos made by Kirill, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the descriptions of Arkady's photos, one per line. Each of these lines contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>k</i></span>), meaning that among coins from the <span class="tex-span"><i>l</i></span>-th to the <span class="tex-span"><i>r</i></span>-th there should be at least one with obverse side up.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the descriptions of Kirill's photos, one per line. Each of these lines contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>k</i></span>), meaning that among coins from the <span class="tex-span"><i>l</i></span>-th to the <span class="tex-span"><i>r</i></span>-th there should be at least one with reverse side up.</p></div><div class="output-specification"><p>Print the only line&nbsp;— the number of ways to choose the side for each coin modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7 = 1000000007</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the total number of coins, the number of photos made by Arkady, and the number of photos made by Kirill, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the descriptions of Arkady's photos, one per line. Each of these lines contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>k</i></span>), meaning that among coins from the <span class="tex-span"><i>l</i></span>-th to the <span class="tex-span"><i>r</i></span>-th there should be at least one with obverse side up.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the descriptions of Kirill's photos, one per line. Each of these lines contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>k</i></span>), meaning that among coins from the <span class="tex-span"><i>l</i></span>-th to the <span class="tex-span"><i>r</i></span>-th there should be at least one with reverse side up.</p>

## Output

<p>Print the only line&nbsp;— the number of ways to choose the side for each coin modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7 = 1000000007</span>.</p>





```input1
5 2 2
1 3
3 5
2 2
4 5

```




```input2
5 3 2
1 3
2 2
3 5
2 2
4 5

```




```input3
60 5 7
1 3
50 60
1 60
30 45
20 40
4 5
6 37
5 18
50 55
22 27
25 31
44 45

```




```output1
8

```




```output2
0

```




```output3
732658600

```



## Note

<p>In the first example the following ways are possible ('<span class="tex-font-style-tt">O</span>'&nbsp;— obverse, '<span class="tex-font-style-tt">R</span>'&nbsp;— reverse side): </p><ul> <li> <span class="tex-font-style-tt">OROOR</span>, </li><li> <span class="tex-font-style-tt">ORORO</span>, </li><li> <span class="tex-font-style-tt">ORORR</span>, </li><li> <span class="tex-font-style-tt">RROOR</span>, </li><li> <span class="tex-font-style-tt">RRORO</span>, </li><li> <span class="tex-font-style-tt">RRORR</span>, </li><li> <span class="tex-font-style-tt">ORROR</span>, </li><li> <span class="tex-font-style-tt">ORRRO</span>. </li></ul><p>In the second example the information is contradictory: the second coin should have obverse and reverse sides up at the same time, that is impossible. So, the answer is <span class="tex-span">0</span>.</p>
