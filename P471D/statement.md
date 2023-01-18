## Description

<div><p>Polar bears Menshykov and Uslada from the zoo of St. Petersburg and elephant Horace from the zoo of Kiev got hold of lots of wooden cubes somewhere. They started making cube towers by placing the cubes one on top of the other. They defined multiple towers standing in a line as a wall. A wall can consist of towers of different heights.</p><p>Horace was the first to finish making his wall. He called his wall an elephant. The wall consists of <span class="tex-span"><i>w</i></span> towers. The bears also finished making their wall but they didn't give it a name. Their wall consists of <span class="tex-span"><i>n</i></span> towers. Horace looked at the bears' tower and wondered: in how many parts of the wall can he "see an elephant"? He can "see an elephant" on a segment of <span class="tex-span"><i>w</i></span> contiguous towers if the heights of the towers on the segment match as a sequence the heights of the towers in Horace's wall. In order to see as many elephants as possible, Horace can raise and lower his wall. He even can lower the wall below the ground level (see the pictures to the samples for clarification).</p><p>Your task is to count the number of segments where Horace can "see an elephant".</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>w</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of towers in the bears' and the elephant's walls correspondingly. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the heights of the towers in the bears' wall. The third line contains <span class="tex-span"><i>w</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the heights of the towers in the elephant's wall.</p></div><div class="output-specification"><p>Print the number of segments in the bears' wall where Horace can "see an elephant".</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>w</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of towers in the bears' and the elephant's walls correspondingly. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the heights of the towers in the bears' wall. The third line contains <span class="tex-span"><i>w</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the heights of the towers in the elephant's wall.</p>

## Output

<p>Print the number of segments in the bears' wall where Horace can "see an elephant".</p>





```input1
13 5
2 4 5 5 4 3 2 2 2 3 3 2 1
3 4 4 3 2

```




```output1
2
```



## Note

<p>The picture to the left shows Horace's wall from the sample, the picture to the right shows the bears' wall. The segments where Horace can "see an elephant" are in gray.</p><center> <img class="tex-graphics" src="file://y2p1Gmi8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
