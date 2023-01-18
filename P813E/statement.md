## Description

<div><p>As you might remember from our previous rounds, Vova really likes computer games. Now he is playing a strategy game known as Rage of Empires.</p><p>In the game Vova can hire <span class="tex-span"><i>n</i></span> different warriors; <span class="tex-span"><i>i</i></span>th warrior has the type <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Vova wants to create a <span class="tex-font-style-it">balanced</span> army hiring some subset of warriors. An army is called <span class="tex-font-style-it">balanced</span> if for each type of warrior present in the game there are not more than <span class="tex-span"><i>k</i></span> warriors of this type in the army. Of course, Vova wants his army to be as large as possible.</p><p>To make things more complicated, Vova has to consider <span class="tex-span"><i>q</i></span> different plans of creating his army. <span class="tex-span"><i>i</i></span>th plan allows him to hire only warriors whose numbers are not less than <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and not greater than <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Help Vova to determine the largest size of a <span class="tex-font-style-it">balanced</span> army for each plan.</p><p><span class="tex-font-style-bf">Be aware that the plans are given in a modified way. See input section for details.</span></p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ... <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100000</span>).</p><p>The third line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100000</span>).</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. <span class="tex-span"><i>i</i></span>th line contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> which represent <span class="tex-span"><i>i</i></span>th plan (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p>You have to keep track of the answer to the last plan (let's call it <span class="tex-span"><i>last</i></span>). In the beginning <span class="tex-span"><i>last</i> = 0</span>. Then to restore values of <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> for the <span class="tex-span"><i>i</i></span>th plan, you have to do the following:</p><ol> <li> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = ((<i>x</i><sub class="lower-index"><i>i</i></sub> + <i>last</i>)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1</span>; </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = ((<i>y</i><sub class="lower-index"><i>i</i></sub> + <i>last</i>)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1</span>; </li><li> If <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> &gt; <i>r</i><sub class="lower-index"><i>i</i></sub></span>, swap <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. </li></ol></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> numbers. <span class="tex-span"><i>i</i></span>th number must be equal to the maximum size of a <span class="tex-font-style-it">balanced</span> army when considering <span class="tex-span"><i>i</i></span>th plan.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ... <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100000</span>).</p><p>The third line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100000</span>).</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. <span class="tex-span"><i>i</i></span>th line contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> which represent <span class="tex-span"><i>i</i></span>th plan (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p>You have to keep track of the answer to the last plan (let's call it <span class="tex-span"><i>last</i></span>). In the beginning <span class="tex-span"><i>last</i> = 0</span>. Then to restore values of <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> for the <span class="tex-span"><i>i</i></span>th plan, you have to do the following:</p><ol> <li> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = ((<i>x</i><sub class="lower-index"><i>i</i></sub> + <i>last</i>)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1</span>; </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = ((<i>y</i><sub class="lower-index"><i>i</i></sub> + <i>last</i>)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1</span>; </li><li> If <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> &gt; <i>r</i><sub class="lower-index"><i>i</i></sub></span>, swap <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. </li></ol>

## Output

<p>Print <span class="tex-span"><i>q</i></span> numbers. <span class="tex-span"><i>i</i></span>th number must be equal to the maximum size of a <span class="tex-font-style-it">balanced</span> army when considering <span class="tex-span"><i>i</i></span>th plan.</p>





```input1
6 2
1 1 1 2 2 2
5
1 6
4 3
1 1
2 6
2 6

```




```output1
2
4
1
3
2

```



## Note

<p>In the first example the real plans are: </p><ol> <li> <span class="tex-span">1&nbsp;2</span> </li><li> <span class="tex-span">1&nbsp;6</span> </li><li> <span class="tex-span">6&nbsp;6</span> </li><li> <span class="tex-span">2&nbsp;4</span> </li><li> <span class="tex-span">4&nbsp;6</span> </li></ol>
