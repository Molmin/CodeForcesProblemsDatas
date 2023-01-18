## Description

<div><p>Polycarp is a music editor at the radio station. He received a playlist for tomorrow, that can be represented as a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is a band, which performs the <span class="tex-span"><i>i</i></span>-th song. Polycarp likes bands with the numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>, but he doesn't really like others. </p><p>We define as <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> the number of songs the group <span class="tex-span"><i>j</i></span> is going to perform tomorrow. Polycarp wants to change the playlist in such a way that the minimum among the numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> will be as large as possible.</p><p>Find this maximum possible value of the minimum among the <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>), and the minimum number of changes in the playlist Polycarp needs to make to achieve it. One change in the playlist is a replacement of the performer of the <span class="tex-span"><i>i</i></span>-th song with any other group.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 2000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the performer of the <span class="tex-span"><i>i</i></span>-th song.</p></div><div class="output-specification"><p>In the first line print two integers: the maximum possible value of the minimum among the <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> is the number of songs in the changed playlist performed by the <span class="tex-span"><i>j</i></span>-th band, and the minimum number of changes in the playlist Polycarp needs to make.</p><p>In the second line print the changed playlist.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 2000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the performer of the <span class="tex-span"><i>i</i></span>-th song.</p>

## Output

<p>In the first line print two integers: the maximum possible value of the minimum among the <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> is the number of songs in the changed playlist performed by the <span class="tex-span"><i>j</i></span>-th band, and the minimum number of changes in the playlist Polycarp needs to make.</p><p>In the second line print the changed playlist.</p><p>If there are multiple answers, print any of them.</p>





```input1
4 2
1 2 3 2

```




```input2
7 3
1 3 2 2 2 2 1

```




```input3
4 4
1000000000 100 7 1000000000

```




```output1
2 1
1 2 1 2 

```




```output2
2 1
1 3 3 2 2 2 1 

```




```output3
1 4
1 2 3 4 

```



## Note

<p>In the first sample, after Polycarp's changes the first band performs two songs (<span class="tex-span"><i>b</i><sub class="lower-index">1</sub> = 2</span>), and the second band also performs two songs (<span class="tex-span"><i>b</i><sub class="lower-index">2</sub> = 2</span>). Thus, the minimum of these values equals to <span class="tex-span">2</span>. It is impossible to achieve a higher minimum value by any changes in the playlist. </p><p>In the second sample, after Polycarp's changes the first band performs two songs (<span class="tex-span"><i>b</i><sub class="lower-index">1</sub> = 2</span>), the second band performs three songs (<span class="tex-span"><i>b</i><sub class="lower-index">2</sub> = 3</span>), and the third band also performs two songs (<span class="tex-span"><i>b</i><sub class="lower-index">3</sub> = 2</span>). Thus, the best minimum value is <span class="tex-span">2</span>. </p>
