## Description

<div><p>Famil Door wants to celebrate his birthday with his friends from Far Far Away. He has <span class="tex-span"><i>n</i></span> friends and each of them can come to the party in a specific range of days of the year from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Of course, Famil Door wants to have as many friends celebrating together with him as possible.</p><p>Far cars are as weird as Far Far Away citizens, so they can only carry two people of opposite gender, that is exactly one male and one female. However, Far is so far from here that no other transportation may be used to get to the party.</p><p>Famil Door should select some day of the year and invite some of his friends, such that they all are available at this moment and the number of male friends invited is equal to the number of female friends invited. Find the maximum number of friends that may present at the party.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— then number of Famil Door's friends.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, that describe the friends. Each line starts with a capital letter '<span class="tex-font-style-tt">F</span>' for female friends and with a capital letter '<span class="tex-font-style-tt">M</span>' for male friends. Then follow two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 366</span>), providing that the <span class="tex-span"><i>i</i></span>-th friend can come to the party from day <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to day <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> inclusive.</p></div><div class="output-specification"><p>Print the maximum number of people that may come to Famil Door's party.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— then number of Famil Door's friends.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, that describe the friends. Each line starts with a capital letter '<span class="tex-font-style-tt">F</span>' for female friends and with a capital letter '<span class="tex-font-style-tt">M</span>' for male friends. Then follow two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 366</span>), providing that the <span class="tex-span"><i>i</i></span>-th friend can come to the party from day <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to day <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> inclusive.</p>

## Output

<p>Print the maximum number of people that may come to Famil Door's party.</p>





```input1
4
M 151 307
F 343 352
F 117 145
M 24 128

```




```input2
6
M 128 130
F 128 131
F 131 140
F 131 141
M 131 200
M 140 200

```




```output1
2

```




```output2
4

```



## Note

<p>In the first sample, friends <span class="tex-span">3</span> and <span class="tex-span">4</span> can come on any day in range <span class="tex-span">[117, 128]</span>.</p><p>In the second sample, friends with indices <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span> can come on day <span class="tex-span">140</span>.</p>
