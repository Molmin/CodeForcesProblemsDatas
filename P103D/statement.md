## Description

<div><p>As you know, the most intelligent beings on the Earth are, of course, cows. This conclusion was reached long ago by the Martian aliens, as well as a number of other intelligent civilizations from outer space. </p><p>Sometimes cows gather into <span class="tex-font-style-it">cowavans</span>. This seems to be seasonal. But at this time the cows become passive and react poorly to external stimuli. A cowavan is a perfect target for the Martian scientific saucer, it's time for large-scale abductions, or, as the Martians say, raids. Simply put, a cowavan is a set of cows in a row. </p><p>If we number all cows in the cowavan with positive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, then we can formalize the popular model of abduction, known as the <span class="tex-font-style-it"><span class="tex-span">(<i>a</i>, <i>b</i>)</span>-Cowavan Raid</span>: first they steal a cow number <span class="tex-span"><i>a</i></span>, then number <span class="tex-span"><i>a</i> + <i>b</i></span>, then — number <span class="tex-span"><i>a</i> + 2·<i>b</i></span>, and so on, until the number of an abducted cow exceeds <span class="tex-span"><i>n</i></span>. During one raid the cows are not renumbered. </p><p>The aliens would be happy to place all the cows on board of their hospitable ship, but unfortunately, the amount of cargo space is very, very limited. The researchers, knowing the mass of each cow in the cowavan, made <span class="tex-span"><i>p</i></span> scenarios of the <span class="tex-span">(<i>a</i>, <i>b</i>)</span>-raid. Now they want to identify the following thing for each scenario individually: what total mass of pure beef will get on board of the ship. All the scenarios are independent, in the process of performing the calculations the cows are not being stolen. </p><center> <img class="tex-graphics" src="file://pni9r3M9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The first line contains the only positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of cows in the cowavan.</p><p>The second number contains <span class="tex-span"><i>n</i></span> positive integer <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, separated by spaces, where the <span class="tex-span"><i>i</i></span>-th number describes the mass of the <span class="tex-span"><i>i</i></span>-th cow in the cowavan (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains the only positive integer <span class="tex-span"><i>p</i></span> — the number of scenarios of <span class="tex-span">(<i>a</i>, <i>b</i>)</span>-raids (<span class="tex-span">1 ≤ <i>p</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>Each following line contains integer parameters <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of the corresponding scenario (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print for each scenario of the <span class="tex-span">(<i>a</i>, <i>b</i>)</span>-raid the total mass of cows, that can be stolen using only this scenario.</p><p>Please, do not use the %lld specificator to read or write 64-bit integers in С++. It is recommended to use the cin, cout streams of the %I64d specificator.</p></div>

## Input

<p>The first line contains the only positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of cows in the cowavan.</p><p>The second number contains <span class="tex-span"><i>n</i></span> positive integer <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, separated by spaces, where the <span class="tex-span"><i>i</i></span>-th number describes the mass of the <span class="tex-span"><i>i</i></span>-th cow in the cowavan (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains the only positive integer <span class="tex-span"><i>p</i></span> — the number of scenarios of <span class="tex-span">(<i>a</i>, <i>b</i>)</span>-raids (<span class="tex-span">1 ≤ <i>p</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>Each following line contains integer parameters <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of the corresponding scenario (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print for each scenario of the <span class="tex-span">(<i>a</i>, <i>b</i>)</span>-raid the total mass of cows, that can be stolen using only this scenario.</p><p>Please, do not use the %lld specificator to read or write 64-bit integers in С++. It is recommended to use the cin, cout streams of the %I64d specificator.</p>





```input1
3
1 2 3
2
1 1
1 2

```




```input2
4
2 3 5 7
3
1 3
2 3
2 2

```




```output1
6
4

```




```output2
9
3
10

```


