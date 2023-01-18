## Description

<div><p>Ivan Anatolyevich's agency is starting to become famous in the town. </p><p>They have already ordered and made <span class="tex-span"><i>n</i></span> TV commercial videos. Each video is made in a special way: the colors and the soundtrack are adjusted to the time of the day and the viewers' mood. That's why the <span class="tex-span"><i>i</i></span>-th video can only be shown within the time range of <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> (it is not necessary to use the whole segment but the broadcast time should be within this segment).</p><p>Now it's time to choose a TV channel to broadcast the commercial. Overall, there are <span class="tex-span"><i>m</i></span> TV channels broadcasting in the city, the <span class="tex-span"><i>j</i></span>-th one has <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> viewers, and is ready to sell time <span class="tex-span">[<i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub>]</span> to broadcast the commercial.</p><p>Ivan Anatolyevich is facing a hard choice: he has to choose exactly one video <span class="tex-span"><i>i</i></span> and exactly one TV channel <span class="tex-span"><i>j</i></span> to broadcast this video and also a time range to broadcast <span class="tex-span">[<i>x</i>, <i>y</i>]</span>. At that the time range should be chosen so that it is both within range <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> and within range <span class="tex-span">[<i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub>]</span>.</p><p>Let's define the <span class="tex-font-style-it">efficiency</span> of the broadcast as value <span class="tex-span">(<i>y</i> - <i>x</i>)·<i>c</i><sub class="lower-index"><i>j</i></sub></span> — the total sum of time that all the viewers of the TV channel are going to spend watching the commercial. Help Ivan Anatolyevich choose the broadcast with the maximum <span class="tex-font-style-it">efficiency</span>!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of commercial videos and channels, respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the segment of time when it is possible to show the corresponding video.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), characterizing the TV channel.</p></div><div class="output-specification"><p>In the first line print an integer — the maximum possible <span class="tex-font-style-it">efficiency</span> of the broadcast. If there is no correct way to get a strictly positive <span class="tex-font-style-it">efficiency</span>, print a zero.</p><p>If the maximum <span class="tex-font-style-it">efficiency</span> is <span class="tex-font-style-bf">strictly</span> positive, in the second line also print the number of the video <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) and the number of the TV channel <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>) in the most effective broadcast.</p><p>If there are multiple optimal answers, you can print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of commercial videos and channels, respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the segment of time when it is possible to show the corresponding video.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), characterizing the TV channel.</p>

## Output

<p>In the first line print an integer — the maximum possible <span class="tex-font-style-it">efficiency</span> of the broadcast. If there is no correct way to get a strictly positive <span class="tex-font-style-it">efficiency</span>, print a zero.</p><p>If the maximum <span class="tex-font-style-it">efficiency</span> is <span class="tex-font-style-bf">strictly</span> positive, in the second line also print the number of the video <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) and the number of the TV channel <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>) in the most effective broadcast.</p><p>If there are multiple optimal answers, you can print any of them.</p>





```input1
2 3
7 9
1 4
2 8 2
0 4 1
8 9 3

```




```input2
1 1
0 0
1 1 10

```




```output1
4
2 1

```




```output2
0

```



## Note

<p>In the first sample test the most optimal solution is to show the second commercial using the first TV channel at time <span class="tex-span">[2, 4]</span>. The efficiency of such solution is equal to <span class="tex-span">(4 - 2)·2 = 4</span>.</p><p>In the second sample test Ivan Anatolievich's wish does not meet the options of the TV channel, the segments do not intersect, so the answer is zero.</p>
