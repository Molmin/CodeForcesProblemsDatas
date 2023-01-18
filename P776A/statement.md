## Description

<div><p>Our beloved detective, Sherlock is currently trying to catch a serial killer who kills a person each day. Using his powers of deduction, he came to know that the killer has a strategy for selecting his next victim.</p><p>The killer starts with two potential victims on his first day, selects one of these two, kills selected victim and replaces him with a new person. He repeats this procedure each day. This way, each day he has two potential victims to choose from. Sherlock knows the initial two potential victims. Also, he knows the murder that happened on a particular day and the new person who replaced this victim.</p><p>You need to help him get all the pairs of potential victims at each day so that Sherlock can observe some pattern.</p></div><div class="input-specification"><p>First line of input contains two names (length of each of them doesn't exceed <span class="tex-span">10</span>), the two initials potential victims. Next line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>), the number of days.</p><p>Next <span class="tex-span"><i>n</i></span> lines contains two names (length of each of them doesn't exceed <span class="tex-span">10</span>), first being the person murdered on this day and the second being the one who replaced that person.</p><p>The input format is consistent, that is, a person murdered is guaranteed to be from the two potential victims at that time. Also, all the names are guaranteed to be distinct and consists of lowercase English letters.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i> + 1</span> lines, the <span class="tex-span"><i>i</i></span>-th line should contain the two persons from which the killer selects for the <span class="tex-span"><i>i</i></span>-th murder. The <span class="tex-span">(<i>n</i> + 1)</span>-th line should contain the two persons from which the next victim is selected. In each line, the two names can be printed in any order.</p></div>

## Input

<p>First line of input contains two names (length of each of them doesn't exceed <span class="tex-span">10</span>), the two initials potential victims. Next line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>), the number of days.</p><p>Next <span class="tex-span"><i>n</i></span> lines contains two names (length of each of them doesn't exceed <span class="tex-span">10</span>), first being the person murdered on this day and the second being the one who replaced that person.</p><p>The input format is consistent, that is, a person murdered is guaranteed to be from the two potential victims at that time. Also, all the names are guaranteed to be distinct and consists of lowercase English letters.</p>

## Output

<p>Output <span class="tex-span"><i>n</i> + 1</span> lines, the <span class="tex-span"><i>i</i></span>-th line should contain the two persons from which the killer selects for the <span class="tex-span"><i>i</i></span>-th murder. The <span class="tex-span">(<i>n</i> + 1)</span>-th line should contain the two persons from which the next victim is selected. In each line, the two names can be printed in any order.</p>





```input1
ross rachel
4
ross joey
rachel phoebe
phoebe monica
monica chandler

```




```input2
icm codeforces
1
codeforces technex

```




```output1
ross rachel
joey rachel
joey phoebe
joey monica
joey chandler

```




```output2
icm codeforces
icm technex

```



## Note

<p>In first example, the killer starts with <span class="tex-font-style-tt">ross</span> and <span class="tex-font-style-tt">rachel</span>. </p><ul> <li> After day <span class="tex-span">1</span>, <span class="tex-font-style-tt">ross</span> is killed and <span class="tex-font-style-tt">joey</span> appears. </li><li> After day <span class="tex-span">2</span>, <span class="tex-font-style-tt">rachel</span> is killed and <span class="tex-font-style-tt">phoebe</span> appears. </li><li> After day <span class="tex-span">3</span>, <span class="tex-font-style-tt">phoebe</span> is killed and <span class="tex-font-style-tt">monica</span> appears. </li><li> After day <span class="tex-span">4</span>, <span class="tex-font-style-tt">monica</span> is killed and <span class="tex-font-style-tt">chandler</span> appears. </li></ul>
