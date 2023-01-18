## Description

<div><p>Only <span class="tex-span"><i>T</i></span> milliseconds left before the start of well-known online programming contest Codehorses Round 2017.</p><p>Polycarp needs to download B++ compiler to take part in the contest. The size of the file is <span class="tex-span"><i>f</i></span> bytes.</p><p>Polycarp's internet tariff allows to download data at the rate of one byte per <span class="tex-span"><i>t</i><sub class="lower-index">0</sub></span> milliseconds. This tariff is already prepaid, and its use does not incur any expense for Polycarp. In addition, the Internet service provider offers two additional packages:</p><ul> <li> download <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> bytes at the rate of one byte per <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> milliseconds, paying <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> burles for the package; </li><li> download <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> bytes at the rate of one byte per <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> milliseconds, paying <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> burles for the package. </li></ul><p>Polycarp can buy any package many times. When buying a package, its price (<span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> or <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>) is prepaid before usage. Once a package is bought it replaces the regular tariff until package data limit is completely used. After a package is consumed Polycarp can immediately buy a new package or switch to the regular tariff without loosing any time. While a package is in use Polycarp can't buy another package or switch back to the regular internet tariff.</p><p>Find the minimum amount of money Polycarp has to spend to download an <span class="tex-span"><i>f</i></span> bytes file no more than in <span class="tex-span"><i>T</i></span> milliseconds.</p><p>Note that because of technical reasons Polycarp can download only integer number of bytes using regular tariff and both packages. I.e. in each of three downloading modes the number of downloaded bytes will be integer. It means that Polycarp can't download a byte partially using the regular tariff or/and both packages.</p></div><div class="input-specification"><p>The first line contains three integer numbers <span class="tex-span"><i>f</i></span>, <span class="tex-span"><i>T</i></span> and <span class="tex-span"><i>t</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>f</i>, <i>T</i>, <i>t</i><sub class="lower-index">0</sub> ≤ 10<sup class="upper-index">7</sup></span>) — size of the file to download (in bytes), maximal time to download the file (in milliseconds) and number of milliseconds to download one byte using the regular internet tariff.</p><p>The second line contains a description of the first additional package. The line contains three integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">7</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> is maximal sizes of downloaded data (in bytes), <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> is time to download one byte (in milliseconds), <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> is price of the package (in burles).</p><p>The third line contains a description of the second additional package. The line contains three integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">7</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> is maximal sizes of downloaded data (in bytes), <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> is time to download one byte (in milliseconds), <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> is price of the package (in burles).</p><p>Polycarp can buy any package many times. Once package is bought it replaces the regular tariff until package data limit is completely used. While a package is in use Polycarp can't buy another package or switch back to the regular internet tariff.</p></div><div class="output-specification"><p>Print the minimum amount of money that Polycarp needs to pay to download B++ compiler no more than in <span class="tex-span"><i>T</i></span> milliseconds. If there is no solution, print the only integer <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains three integer numbers <span class="tex-span"><i>f</i></span>, <span class="tex-span"><i>T</i></span> and <span class="tex-span"><i>t</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>f</i>, <i>T</i>, <i>t</i><sub class="lower-index">0</sub> ≤ 10<sup class="upper-index">7</sup></span>) — size of the file to download (in bytes), maximal time to download the file (in milliseconds) and number of milliseconds to download one byte using the regular internet tariff.</p><p>The second line contains a description of the first additional package. The line contains three integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">7</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> is maximal sizes of downloaded data (in bytes), <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> is time to download one byte (in milliseconds), <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> is price of the package (in burles).</p><p>The third line contains a description of the second additional package. The line contains three integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">7</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> is maximal sizes of downloaded data (in bytes), <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> is time to download one byte (in milliseconds), <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> is price of the package (in burles).</p><p>Polycarp can buy any package many times. Once package is bought it replaces the regular tariff until package data limit is completely used. While a package is in use Polycarp can't buy another package or switch back to the regular internet tariff.</p>

## Output

<p>Print the minimum amount of money that Polycarp needs to pay to download B++ compiler no more than in <span class="tex-span"><i>T</i></span> milliseconds. If there is no solution, print the only integer <span class="tex-font-style-tt">-1</span>.</p>





```input1
120 964 20
26 8 8
13 10 4

```




```input2
10 200 20
1 1 1
2 2 3

```




```input3
8 81 11
4 10 16
3 10 12

```




```input4
8 79 11
4 10 16
3 10 12

```




```output1
40

```




```output2
0

```




```output3
28

```




```output4
-1

```



## Note

<p>In the first example Polycarp has to buy the first additional package 5 times and do not buy the second additional package. He downloads 120 bytes (of total <span class="tex-span">26·5 = 130</span> bytes) in <span class="tex-span">120·8 = 960</span> milliseconds (<span class="tex-span">960 ≤ 964</span>). He spends <span class="tex-span">8·5 = 40</span> burles on it.</p><p>In the second example Polycarp has enough time to download <span class="tex-span">10</span> bytes. It takes <span class="tex-span">10·20 = 200</span> milliseconds which equals to upper constraint on download time.</p><p>In the third example Polycarp has to buy one first additional package and one second additional package.</p><p>In the fourth example Polycarp has no way to download the file on time.</p>
