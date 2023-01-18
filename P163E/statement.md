## Description

<div><p>The best programmers of Embezzland compete to develop a part of the project called "e-Government" — the system of automated statistic collecting and press analysis.</p><p>We know that any of the <span class="tex-span"><i>k</i></span> citizens can become a member of the Embezzland government. The citizens' surnames are <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>. All surnames are different. Initially all <span class="tex-span"><i>k</i></span> citizens from this list are members of the government. The system should support the following options:</p><ul> <li> Include citizen <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to the government. </li><li> Exclude citizen <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> from the government. </li><li> Given a newspaper article text, calculate how politicized it is. To do this, for every active government member the system counts the number of times his surname occurs in the text as a substring. All occurrences are taken into consideration, including the intersecting ones. The degree of politicization of a text is defined as the sum of these values for all active government members. </li></ul><p>Implement this system.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries to the system and the number of potential government members.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain the surnames <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>, one per line. All surnames are pairwise different.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain queries to the system, one per line. Each query consists of a character that determines an operation and the operation argument, written consecutively without a space.</p><p>Operation "include in the government" corresponds to the character "<span class="tex-font-style-tt">+</span>", operation "exclude" corresponds to "<span class="tex-font-style-tt">-</span>". An argument of those operations is an integer between <span class="tex-span">1</span> and <span class="tex-span"><i>k</i></span> — the index of the citizen involved in the operation. Any citizen can be included and excluded from the government an arbitrary number of times in any order. Including in the government a citizen who is already there or excluding the citizen who isn't there changes nothing.</p><p>The operation "calculate politicization" corresponds to character "<span class="tex-font-style-tt">?</span>". Its argument is a text.</p><p>All strings — surnames and texts — are non-empty sequences of lowercase Latin letters. The total length of all surnames doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>, the total length of all texts doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>For any "calculate politicization" operation print on a separate line the degree of the politicization of the given text. Print nothing for other operations.</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries to the system and the number of potential government members.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain the surnames <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>, one per line. All surnames are pairwise different.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain queries to the system, one per line. Each query consists of a character that determines an operation and the operation argument, written consecutively without a space.</p><p>Operation "include in the government" corresponds to the character "<span class="tex-font-style-tt">+</span>", operation "exclude" corresponds to "<span class="tex-font-style-tt">-</span>". An argument of those operations is an integer between <span class="tex-span">1</span> and <span class="tex-span"><i>k</i></span> — the index of the citizen involved in the operation. Any citizen can be included and excluded from the government an arbitrary number of times in any order. Including in the government a citizen who is already there or excluding the citizen who isn't there changes nothing.</p><p>The operation "calculate politicization" corresponds to character "<span class="tex-font-style-tt">?</span>". Its argument is a text.</p><p>All strings — surnames and texts — are non-empty sequences of lowercase Latin letters. The total length of all surnames doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>, the total length of all texts doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>For any "calculate politicization" operation print on a separate line the degree of the politicization of the given text. Print nothing for other operations.</p>





```input1
7 3
a
aa
ab
?aaab
-2
?aaab
-3
?aaab
+2
?aabbaa

```




```output1
6
4
3
6

```


