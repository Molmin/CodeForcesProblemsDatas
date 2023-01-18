## Description

<div><p>You have <span class="tex-span"><i>k</i></span> pieces of laundry, each of which you want to wash, dry and fold. You are at a laundromat that has <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> washing machines, <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> drying machines and <span class="tex-span"><i>n</i><sub class="lower-index">3</sub></span> folding machines. Each machine can process only one piece of laundry at a time. You can't dry a piece of laundry before it is washed, and you can't fold it before it is dried. Moreover, after a piece of laundry is washed, it needs to be immediately moved into a drying machine, and after it is dried, it needs to be immediately moved into a folding machine.</p><p>It takes <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> minutes to wash one piece of laundry in a washing machine, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> minutes to dry it in a drying machine, and <span class="tex-span"><i>t</i><sub class="lower-index">3</sub></span> minutes to fold it in a folding machine. Find the smallest number of minutes that is enough to wash, dry and fold all the laundry you have.</p></div><div class="input-specification"><p>The only line of the input contains seven integers: <span class="tex-span"><i>k</i>, <i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub>, <i>n</i><sub class="lower-index">3</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">3</sub></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup>;&nbsp;1 ≤ <i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub>, <i>n</i><sub class="lower-index">3</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">3</sub> ≤ 1000)</span>.</p></div><div class="output-specification"><p>Print one integer — smallest number of minutes to do all your laundry.</p></div>

## Input

<p>The only line of the input contains seven integers: <span class="tex-span"><i>k</i>, <i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub>, <i>n</i><sub class="lower-index">3</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">3</sub></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup>;&nbsp;1 ≤ <i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub>, <i>n</i><sub class="lower-index">3</sub>, <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">3</sub> ≤ 1000)</span>.</p>

## Output

<p>Print one integer — smallest number of minutes to do all your laundry.</p>





```input1
1 1 1 1 5 5 5

```




```input2
8 4 3 2 10 5 2

```




```output1
15

```




```output2
32

```



## Note

<p>In the first example there's one instance of each machine, each taking 5 minutes to complete. You have only one piece of laundry, so it takes 15 minutes to process it.</p><p>In the second example you start washing first two pieces at moment <span class="tex-span">0</span>. If you start the third piece of laundry immediately, then by the time it is dried, there will be no folding machine available, so you have to wait, and start washing third piece at moment <span class="tex-span">2</span>. Similarly, you can't start washing next piece until moment <span class="tex-span">5</span>, since otherwise there will be no dryer available, when it is washed. Start time for each of the eight pieces of laundry is <span class="tex-span">0, 0, 2, 5, 10, 10, 12</span> and <span class="tex-span">15</span> minutes respectively. The last piece of laundry will be ready after <span class="tex-span">15 + 10 + 5 + 2 = 32</span> minutes.</p>
