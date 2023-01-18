## Description

<div><p>Every summer Vitya comes to visit his grandmother in the countryside. This summer, he got a huge wart. Every grandma knows that one should treat warts when the moon goes down. Thus, Vitya has to catch the moment when the moon is down.</p><p>Moon cycle lasts 30 days. The size of the visible part of the moon (in Vitya's units) for each day is <span class="tex-span">0</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">5</span>, <span class="tex-span">6</span>, <span class="tex-span">7</span>, <span class="tex-span">8</span>, <span class="tex-span">9</span>, <span class="tex-span">10</span>, <span class="tex-span">11</span>, <span class="tex-span">12</span>, <span class="tex-span">13</span>, <span class="tex-span">14</span>, <span class="tex-span">15</span>, <span class="tex-span">14</span>, <span class="tex-span">13</span>, <span class="tex-span">12</span>, <span class="tex-span">11</span>, <span class="tex-span">10</span>, <span class="tex-span">9</span>, <span class="tex-span">8</span>, <span class="tex-span">7</span>, <span class="tex-span">6</span>, <span class="tex-span">5</span>, <span class="tex-span">4</span>, <span class="tex-span">3</span>, <span class="tex-span">2</span>, <span class="tex-span">1</span>, and then cycle repeats, thus after the second <span class="tex-span">1</span> again goes <span class="tex-span">0</span>.</p><p>As there is no internet in the countryside, Vitya has been watching the moon for <span class="tex-span"><i>n</i></span> consecutive days and for each of these days he wrote down the size of the visible part of the moon. Help him find out whether the moon will be up or down next day, or this cannot be determined by the data he has.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 92</span>)&nbsp;— the number of consecutive days Vitya was watching the size of the visible part of the moon. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 15</span>)&nbsp;— Vitya's records.</p><p>It's guaranteed that the input data is consistent.</p></div><div class="output-specification"><p>If Vitya can be sure that the size of visible part of the moon on day <span class="tex-span"><i>n</i> + 1</span> will be less than the size of the visible part on day <span class="tex-span"><i>n</i></span>, then print "<span class="tex-font-style-tt">DOWN</span>" at the only line of the output. If he might be sure that the size of the visible part will increase, then print "<span class="tex-font-style-tt">UP</span>". If it's impossible to determine what exactly will happen with the moon, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 92</span>)&nbsp;— the number of consecutive days Vitya was watching the size of the visible part of the moon. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 15</span>)&nbsp;— Vitya's records.</p><p>It's guaranteed that the input data is consistent.</p>

## Output

<p>If Vitya can be sure that the size of visible part of the moon on day <span class="tex-span"><i>n</i> + 1</span> will be less than the size of the visible part on day <span class="tex-span"><i>n</i></span>, then print "<span class="tex-font-style-tt">DOWN</span>" at the only line of the output. If he might be sure that the size of the visible part will increase, then print "<span class="tex-font-style-tt">UP</span>". If it's impossible to determine what exactly will happen with the moon, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5
3 4 5 6 7

```




```input2
7
12 13 14 15 14 13 12

```




```input3
1
8

```




```output1
UP

```




```output2
DOWN

```




```output3
-1

```



## Note

<p>In the first sample, the size of the moon on the next day will be equal to <span class="tex-span">8</span>, thus the answer is "<span class="tex-font-style-tt">UP</span>".</p><p>In the second sample, the size of the moon on the next day will be <span class="tex-span">11</span>, thus the answer is "<span class="tex-font-style-tt">DOWN</span>".</p><p>In the third sample, there is no way to determine whether the size of the moon on the next day will be <span class="tex-span">7</span> or <span class="tex-span">9</span>, thus the answer is <span class="tex-font-style-tt">-1</span>.</p>
