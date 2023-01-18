## Description

<div><p>Mr. Kitayuta's garden is planted with <span class="tex-span"><i>n</i></span> bamboos. (Bamboos are tall, fast-growing tropical plants with hollow stems.) At the moment, the height of the <span class="tex-span"><i>i</i></span>-th bamboo is <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> meters, and it grows <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> meters at the end of each day. </p><p>Actually, Mr. Kitayuta hates these bamboos. He once attempted to cut them down, but failed because their stems are too hard. Mr. Kitayuta have not given up, however. He has crafted Magical Hammer with his intelligence to drive them into the ground.</p><p>He can use Magical Hammer at most <span class="tex-span"><i>k</i></span> times during each day, due to his limited Magic Power. Each time he beat a bamboo with Magical Hammer, its height decreases by <span class="tex-span"><i>p</i></span> meters. If the height would become negative by this change, it will become <span class="tex-span">0</span> meters instead (it does not disappear). In other words, if a bamboo whose height is <span class="tex-span"><i>h</i></span> meters is beaten with Magical Hammer, its new height will be <span class="tex-span"><i>max</i>(0, <i>h</i> - <i>p</i>)</span> meters. It is possible to beat the same bamboo more than once in a day.</p><p>Mr. Kitayuta will fight the bamboos for <span class="tex-span"><i>m</i></span> days, starting today. His purpose is to minimize the height of the tallest bamboo after <span class="tex-span"><i>m</i></span> days (that is, <span class="tex-span"><i>m</i></span> iterations of "Mr. Kitayuta beats the bamboos and then they grow"). Find the lowest possible height of the tallest bamboo after <span class="tex-span"><i>m</i></span> days.</p></div><div class="input-specification"><p>The first line of the input contains four space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 5000, 1 ≤ <i>k</i> ≤ 10, 1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>). They represent the number of the bamboos in Mr. Kitayuta's garden, the duration of Mr. Kitayuta's fight in days, the maximum number of times that Mr. Kitayuta beat the bamboos during each day, and the power of Magic Hammer, respectively.</p><p>The following <span class="tex-span"><i>n</i></span> lines describe the properties of the bamboos. The <span class="tex-span"><i>i</i></span>-th of them (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) contains two space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), denoting the initial height and the growth rate of the <span class="tex-span"><i>i</i></span>-th bamboo, respectively.</p></div><div class="output-specification"><p>Print the lowest possible height of the tallest bamboo after <span class="tex-span"><i>m</i></span> days.</p></div>

## Input

<p>The first line of the input contains four space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 5000, 1 ≤ <i>k</i> ≤ 10, 1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>). They represent the number of the bamboos in Mr. Kitayuta's garden, the duration of Mr. Kitayuta's fight in days, the maximum number of times that Mr. Kitayuta beat the bamboos during each day, and the power of Magic Hammer, respectively.</p><p>The following <span class="tex-span"><i>n</i></span> lines describe the properties of the bamboos. The <span class="tex-span"><i>i</i></span>-th of them (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) contains two space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), denoting the initial height and the growth rate of the <span class="tex-span"><i>i</i></span>-th bamboo, respectively.</p>

## Output

<p>Print the lowest possible height of the tallest bamboo after <span class="tex-span"><i>m</i></span> days.</p>





```input1
3 1 2 5
10 10
10 10
15 2

```




```input2
2 10 10 1000000000
0 10
0 10

```




```input3
5 3 3 10
9 5
9 2
4 7
9 10
3 8

```




```output1
17

```




```output2
10

```




```output3
14

```


