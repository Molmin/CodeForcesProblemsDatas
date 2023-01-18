## Description

<div><p>After studying the beacons Mister B decided to visit alien's planet, because he learned that they live in a system of flickering star Moon. Moreover, Mister B learned that the star shines once in exactly <span class="tex-span"><i>T</i></span> seconds. The problem is that the star is yet to be discovered by scientists.</p><p>There are <span class="tex-span"><i>n</i></span> astronomers numerated from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> trying to detect the star. They try to detect the star by sending requests to record the sky for <span class="tex-span">1</span> second. </p><p>The astronomers send requests <span class="tex-font-style-bf">in cycle</span>: the <span class="tex-span"><i>i</i></span>-th astronomer sends a request exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> second after the <span class="tex-span">(<i>i</i> - 1)</span>-th (i.e. if the previous request was sent at moment <span class="tex-span"><i>t</i></span>, then the next request is sent at moment <span class="tex-span"><i>t</i> + <i>a</i><sub class="lower-index"><i>i</i></sub></span>); the <span class="tex-span">1</span>-st astronomer sends requests <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> seconds later than the <span class="tex-span"><i>n</i></span>-th. The first astronomer sends his first request at moment <span class="tex-span">0</span>.</p><p>Mister B doesn't know the first moment the star is going to shine, but it's obvious that all moments at which the star will shine are determined by the time of its shine moment in the interval <span class="tex-span">[0, <i>T</i>)</span>. Moreover, this interval can be split into <span class="tex-span"><i>T</i></span> parts of <span class="tex-span">1</span> second length each of form <span class="tex-span">[<i>t</i>, <i>t</i> + 1)</span>, where <span class="tex-span"><i>t</i> = 0, 1, 2, ..., (<i>T</i> - 1)</span>.</p><p>Mister B wants to know how lucky each astronomer can be in discovering the star first.</p><p>For each astronomer compute how many segments of form <span class="tex-span">[<i>t</i>, <i>t</i> + 1)</span> (<span class="tex-span"><i>t</i> = 0, 1, 2, ..., (<i>T</i> - 1)</span>) there are in the interval <span class="tex-span">[0, <i>T</i>)</span> so that this astronomer is the first to discover the star if the first shine of the star happens in this time interval.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>T</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers: for each astronomer print the number of time segments describer earlier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>T</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers: for each astronomer print the number of time segments describer earlier.</p>





```input1
4 2
2 3

```




```input2
5 4
1 1 1 1

```




```output1
3 1 

```




```output2
2 1 1 1 

```



## Note

<p>In the first sample test the first astronomer will send requests at moments <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> = 0, 5, 10, ...</span>, the second — at moments <span class="tex-span"><i>t</i><sub class="lower-index">2</sub> = 3, 8, 13, ...</span>. That's why interval <span class="tex-span">[0, 1)</span> the first astronomer will discover first at moment <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> = 0</span>, <span class="tex-span">[1, 2)</span> — the first astronomer at moment <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> = 5</span>, <span class="tex-span">[2, 3)</span> — the first astronomer at moment <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> = 10</span>, and <span class="tex-span">[3, 4)</span> — the second astronomer at moment <span class="tex-span"><i>t</i><sub class="lower-index">2</sub> = 3</span>.</p><p>In the second sample test interval <span class="tex-span">[0, 1)</span> — the first astronomer will discover first, <span class="tex-span">[1, 2)</span> — the second astronomer, <span class="tex-span">[2, 3)</span> — the third astronomer, <span class="tex-span">[3, 4)</span> — the fourth astronomer, <span class="tex-span">[4, 5)</span> — the first astronomer.</p>
