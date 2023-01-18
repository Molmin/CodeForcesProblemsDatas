## Description

<div><p>In Arcady's garden there grows a peculiar apple-tree that fruits one time per year. Its peculiarity can be explained in following way: there are <span class="tex-span"><i>n</i></span> inflorescences, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Inflorescence number <span class="tex-span">1</span> is situated near base of tree and any other inflorescence with number <span class="tex-span"><i>i</i></span> (<span class="tex-span"><i>i</i> &gt; 1</span>) is situated at the top of branch, which bottom is <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>-th inflorescence and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>.</p><p>Once tree starts fruiting, there appears exactly one apple in each inflorescence. The same moment as apples appear, they start to roll down along branches to the very base of tree. Each second all apples, except ones in first inflorescence simultaneously roll down one branch closer to tree base, e.g. apple in <span class="tex-span"><i>a</i></span>-th inflorescence gets to <span class="tex-span"><i>p</i><sub class="lower-index"><i>a</i></sub></span>-th inflorescence. Apples that end up in first inflorescence are gathered by Arcady in exactly the same moment. Second peculiarity of this tree is that once two apples are in same inflorescence they <span class="tex-font-style-bf">annihilate</span>. This happens with each pair of apples, e.g. if there are <span class="tex-span">5</span> apples in same inflorescence in same time, only one will not be annihilated and if there are <span class="tex-span">8</span> apples, all apples will be annihilated. Thus, there can be no more than one apple in each inflorescence in each moment of time.</p><p>Help Arcady with counting number of apples he will be able to collect from first inflorescence during one harvest.</p></div><div class="input-specification"><p>First line of input contains single integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) &nbsp;— number of inflorescences.</p><p>Second line of input contains sequence of <span class="tex-span"><i>n</i> - 1</span> integer numbers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is number of inflorescence into which the apple from <span class="tex-span"><i>i</i></span>-th inflorescence rolls down.</p></div><div class="output-specification"><p>Single line of output should contain one integer number: amount of apples that Arcady will be able to collect from first inflorescence during one harvest.</p></div>

## Input

<p>First line of input contains single integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) &nbsp;— number of inflorescences.</p><p>Second line of input contains sequence of <span class="tex-span"><i>n</i> - 1</span> integer numbers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is number of inflorescence into which the apple from <span class="tex-span"><i>i</i></span>-th inflorescence rolls down.</p>

## Output

<p>Single line of output should contain one integer number: amount of apples that Arcady will be able to collect from first inflorescence during one harvest.</p>





```input1
3
1 1

```




```input2
5
1 2 2 2

```




```input3
18
1 1 1 4 4 3 2 2 2 10 8 9 9 9 10 10 4

```




```output1
1

```




```output2
3

```




```output3
4

```



## Note

<p>In first example Arcady will be able to collect only one apple, initially situated in <span class="tex-span">1</span>st inflorescence. In next second apples from <span class="tex-span">2</span>nd and <span class="tex-span">3</span>rd inflorescences will roll down and annihilate, and Arcady won't be able to collect them.</p><p>In the second example Arcady will be able to collect 3 apples. First one is one initially situated in first inflorescence. In a second apple from <span class="tex-span">2</span>nd inflorescence will roll down to <span class="tex-span">1</span>st (Arcady will collect it) and apples from <span class="tex-span">3</span>rd, <span class="tex-span">4</span>th, <span class="tex-span">5</span>th inflorescences will roll down to <span class="tex-span">2</span>nd. Two of them will annihilate and one not annihilated will roll down from <span class="tex-span">2</span>-nd inflorescence to <span class="tex-span">1</span>st one in the next second and Arcady will collect it.</p>
