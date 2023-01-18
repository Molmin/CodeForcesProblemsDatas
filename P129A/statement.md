## Description

<div><p>Olga came to visit the twins Anna and Maria and saw that they have many cookies. The cookies are distributed into bags. As there are many cookies, Olga decided that it's no big deal if she steals a bag. However, she doesn't want the sisters to quarrel because of nothing when they divide the cookies. That's why Olga wants to steal a bag with cookies so that the number of cookies in the remaining bags was even, that is, so that Anna and Maria could evenly divide it into two (even 0 remaining cookies will do, just as any other even number). How many ways there are to steal exactly one cookie bag so that the total number of cookies in the remaining bags was even?</p></div><div class="input-specification"><p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of cookie bags Anna and Maria have. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of cookies in the <span class="tex-span"><i>i</i></span>-th bag.</p></div><div class="output-specification"><p>Print in the only line the only number — the sought number of ways. If there are no such ways print 0.</p></div>

## Input

<p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of cookie bags Anna and Maria have. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of cookies in the <span class="tex-span"><i>i</i></span>-th bag.</p>

## Output

<p>Print in the only line the only number — the sought number of ways. If there are no such ways print 0.</p>





```input1
1
1

```




```input2
10
1 2 2 3 4 4 4 2 2 2

```




```input3
11
2 2 2 2 2 2 2 2 2 2 99

```




```output1
1

```




```output2
8

```




```output3
1

```



## Note

<p>In the first sample Olga should take the only bag so that the twins ended up with the even number of cookies.</p><p>In the second sample Olga can take any of five bags with two cookies or any of three bags with four cookies — <span class="tex-span">5 + 3 = 8</span> ways in total.</p><p>In the third sample, no matter which bag with two cookies Olga chooses, the twins are left with <span class="tex-span">2 * 9 + 99 = 117</span> cookies. Thus, Olga has only one option: to take the bag with <span class="tex-span">99</span> cookies.</p>
