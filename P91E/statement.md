## Description

<div><p>Today the North Pole hosts an Olympiad in a sport called... toy igloo skyscrapers' building!</p><p>There are <span class="tex-span"><i>n</i></span> walruses taking part in the contest. Each walrus is given a unique number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. After start each walrus begins to build his own igloo skyscraper. Initially, at the moment of time equal to <span class="tex-span">0</span>, the height of the skyscraper <span class="tex-span"><i>i</i></span>-th walrus is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Each minute the <span class="tex-span"><i>i</i></span>-th walrus finishes building <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> floors.</p><p>The journalists that are reporting from the spot where the Olympiad is taking place, make <span class="tex-span"><i>q</i></span> queries to the organizers. Each query is characterized by a group of three numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. The organizers respond to each query with a number <span class="tex-span"><i>x</i></span>, such that:</p><p>1. Number <span class="tex-span"><i>x</i></span> lies on the interval from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> inclusive (<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>).</p><p>2. The skyscraper of the walrus number <span class="tex-span"><i>x</i></span> possesses the maximum height among the skyscrapers of all walruses from the interval <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> at the moment of time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>For each journalists' query print the number of the walrus <span class="tex-span"><i>x</i></span> that meets the above-given criteria. If there are several possible answers, print any of them.</p></div><div class="input-specification"><p>The first line contains numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>). Next <span class="tex-span"><i>n</i></span> lines contain pairs of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Then follow <span class="tex-span"><i>q</i></span> queries i the following format <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, one per each line (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). All input numbers are integers.</p></div><div class="output-specification"><p>For each journalists' query print the number of the walrus <span class="tex-span"><i>x</i></span> that meets the criteria, given in the statement. Print one number per line.</p></div>

## Input

<p>The first line contains numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>). Next <span class="tex-span"><i>n</i></span> lines contain pairs of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Then follow <span class="tex-span"><i>q</i></span> queries i the following format <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, one per each line (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). All input numbers are integers.</p>

## Output

<p>For each journalists' query print the number of the walrus <span class="tex-span"><i>x</i></span> that meets the criteria, given in the statement. Print one number per line.</p>





```input1
5 4
4 1
3 5
6 2
3 5
6 5
1 5 2
1 3 5
1 1 0
1 5 0

```




```input2
5 4
6 1
5 1
2 5
4 3
6 1
2 4 1
3 4 5
1 4 5
1 2 0

```




```output1
5
2
1
5

```




```output2
3
3
3
1

```


