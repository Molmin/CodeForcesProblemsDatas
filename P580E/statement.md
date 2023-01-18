## Description

<div><p>One day Kefa the parrot was walking down the street as he was on the way home from the restaurant when he saw something glittering by the road. As he came nearer he understood that it was a watch. He decided to take it to the pawnbroker to earn some money. </p><p>The pawnbroker said that each watch contains a serial number represented by a string of digits from <span class="tex-span">0</span> to <span class="tex-span">9</span>, and the more quality checks this number passes, the higher is the value of the watch. The check is defined by three positive integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>d</i></span>. The watches pass a check if a substring of the serial number from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> has period <span class="tex-span"><i>d</i></span>. Sometimes the pawnbroker gets distracted and Kefa changes in some substring of the serial number all digits to <span class="tex-span"><i>c</i></span> in order to increase profit from the watch. </p><p>The seller has a lot of things to do to begin with and with Kefa messing about, he gave you a task: to write a program that determines the value of the watch.</p><p>Let us remind you that number <span class="tex-span"><i>x</i></span> is called a period of string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ |<i>s</i>|</span>), if <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>  =  <i>s</i><sub class="lower-index"><i>i</i> + <i>x</i></sub></span> for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span">|<i>s</i>|  -  <i>x</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> + <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the serial number, the number of change made by Kefa and the number of quality checks.</p><p>The second line contains a serial number consisting of <span class="tex-span"><i>n</i></span> digits.</p><p>Then <span class="tex-span"><i>m</i> + <i>k</i></span> lines follow, containing either checks or changes. </p><p>The changes are given as 1 <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i> ≤ 9</span>). That means that Kefa changed all the digits from the <span class="tex-span"><i>l</i></span>-th to the <span class="tex-span"><i>r</i></span>-th to be <span class="tex-span"><i>c</i></span>. </p><p>The checks are given as 2 <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>d</i> ≤ <i>r</i> - <i>l</i> + 1</span>).</p></div><div class="output-specification"><p>For each check on a single line print "<span class="tex-font-style-tt">YES</span>" if the watch passed it, otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line of the input contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> + <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the serial number, the number of change made by Kefa and the number of quality checks.</p><p>The second line contains a serial number consisting of <span class="tex-span"><i>n</i></span> digits.</p><p>Then <span class="tex-span"><i>m</i> + <i>k</i></span> lines follow, containing either checks or changes. </p><p>The changes are given as 1 <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i> ≤ 9</span>). That means that Kefa changed all the digits from the <span class="tex-span"><i>l</i></span>-th to the <span class="tex-span"><i>r</i></span>-th to be <span class="tex-span"><i>c</i></span>. </p><p>The checks are given as 2 <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>d</i> ≤ <i>r</i> - <i>l</i> + 1</span>).</p>

## Output

<p>For each check on a single line print "<span class="tex-font-style-tt">YES</span>" if the watch passed it, otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
3 1 2
112
2 2 3 1
1 1 3 8
2 1 2 1

```




```input2
6 2 3
334934
2 2 5 2
1 4 4 3
2 1 6 3
1 2 3 8
2 3 6 1

```




```output1
NO
YES

```




```output2
NO
YES
NO

```



## Note

<p>In the first sample test two checks will be made. In the first one substring "12" is checked on whether or not it has period 1, so the answer is "<span class="tex-font-style-tt">NO</span>". In the second one substring "88", is checked on whether or not it has period 1, and it has this period, so the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>In the second statement test three checks will be made. The first check processes substring "3493", which doesn't have period 2. Before the second check the string looks as "334334", so the answer to it is "<span class="tex-font-style-tt">YES</span>". And finally, the third check processes substring "8334", which does not have period 1.</p>
