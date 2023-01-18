## Description

<div><p>A TV show called "Guess a number!" is gathering popularity. The whole Berland, the old and the young, are watching the show.</p><p>The rules are simple. The host thinks of an integer <span class="tex-span"><i>y</i></span> and the participants guess it by asking questions to the host. There are four types of acceptable questions:</p><ul> <li> Is it true that <span class="tex-span"><i>y</i></span> is strictly larger than number <span class="tex-span"><i>x</i></span>? </li><li> Is it true that <span class="tex-span"><i>y</i></span> is strictly smaller than number <span class="tex-span"><i>x</i></span>? </li><li> Is it true that <span class="tex-span"><i>y</i></span> is larger than or equal to number <span class="tex-span"><i>x</i></span>? </li><li> Is it true that <span class="tex-span"><i>y</i></span> is smaller than or equal to number <span class="tex-span"><i>x</i></span>? </li></ul><p>On each question the host answers truthfully, "yes" or "no".</p><p>Given the sequence of questions and answers, find any integer value of <span class="tex-span"><i>y</i></span> that meets the criteria of all answers. If there isn't such value, print "<span class="tex-font-style-tt">Impossible</span>".</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>) — the number of questions (and answers). Next <span class="tex-span"><i>n</i></span> lines each contain one question and one answer to it. The format of each line is like that: "<span class="tex-font-style-it">sign x answer</span>", where the <span class="tex-font-style-it">sign</span> is:</p><ul> <li> "<span class="tex-font-style-tt">&gt;</span>" (for the first type queries), </li><li> "<span class="tex-font-style-tt">&lt;</span>" (for the second type queries), </li><li> "<span class="tex-font-style-tt">&gt;=</span>" (for the third type queries), </li><li> "<span class="tex-font-style-tt">&lt;=</span>" (for the fourth type queries). </li></ul><p>All values of <span class="tex-span"><i>x</i></span> are integer and meet the inequation <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>. The <span class="tex-font-style-it">answer</span> is an English letter "<span class="tex-font-style-tt">Y</span>" (for "yes") or "<span class="tex-font-style-tt">N</span>" (for "no").</p><p>Consequtive elements in lines are separated by a single space.</p></div><div class="output-specification"><p>Print any of such integers <span class="tex-span"><i>y</i></span>, that the answers to all the queries are correct. The printed number <span class="tex-span"><i>y</i></span> must meet the inequation <span class="tex-span"> - 2·10<sup class="upper-index">9</sup> ≤ <i>y</i> ≤ 2·10<sup class="upper-index">9</sup></span>. If there are many answers, print any of them. If such value doesn't exist, print word "<span class="tex-font-style-tt">Impossible</span>" (without the quotes).</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>) — the number of questions (and answers). Next <span class="tex-span"><i>n</i></span> lines each contain one question and one answer to it. The format of each line is like that: "<span class="tex-font-style-it">sign x answer</span>", where the <span class="tex-font-style-it">sign</span> is:</p><ul> <li> "<span class="tex-font-style-tt">&gt;</span>" (for the first type queries), </li><li> "<span class="tex-font-style-tt">&lt;</span>" (for the second type queries), </li><li> "<span class="tex-font-style-tt">&gt;=</span>" (for the third type queries), </li><li> "<span class="tex-font-style-tt">&lt;=</span>" (for the fourth type queries). </li></ul><p>All values of <span class="tex-span"><i>x</i></span> are integer and meet the inequation <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>. The <span class="tex-font-style-it">answer</span> is an English letter "<span class="tex-font-style-tt">Y</span>" (for "yes") or "<span class="tex-font-style-tt">N</span>" (for "no").</p><p>Consequtive elements in lines are separated by a single space.</p>

## Output

<p>Print any of such integers <span class="tex-span"><i>y</i></span>, that the answers to all the queries are correct. The printed number <span class="tex-span"><i>y</i></span> must meet the inequation <span class="tex-span"> - 2·10<sup class="upper-index">9</sup> ≤ <i>y</i> ≤ 2·10<sup class="upper-index">9</sup></span>. If there are many answers, print any of them. If such value doesn't exist, print word "<span class="tex-font-style-tt">Impossible</span>" (without the quotes).</p>





```input1
4
&gt;= 1 Y
&lt; 3 N
&lt;= -3 N
&gt; 55 N

```




```input2
2
&gt; 100 Y
&lt; -100 Y

```




```output1
17

```




```output2
Impossible

```


