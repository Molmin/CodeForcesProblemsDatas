## Description

<div><p>International Abbreviation Olympiad takes place annually starting from 1989. Each year the competition receives an abbreviation of form <span class="tex-font-style-tt">IAO'y</span>, where <span class="tex-span"><i>y</i></span> stands for some number of consequent last digits of the current year. Organizers always pick an abbreviation with non-empty string <span class="tex-span"><i>y</i></span> that has never been used before. Among all such valid abbreviations they choose the shortest one and announce it to be the abbreviation of this year's competition.</p><p>For example, the first three Olympiads (years 1989, 1990 and 1991, respectively) received the abbreviations <span class="tex-font-style-tt">IAO'9</span>, <span class="tex-font-style-tt">IAO'0</span> and <span class="tex-font-style-tt">IAO'1</span>, while the competition in 2015 received an abbreviation <span class="tex-font-style-tt">IAO'15</span>, as <span class="tex-font-style-tt">IAO'5</span> has been already used in 1995.</p><p>You are given a list of abbreviations. For each of them determine the year it stands for.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of abbreviations to process. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each containing a single abbreviation. It's guaranteed that each abbreviation contains at most nine digits.</p></div><div class="output-specification"><p>For each abbreviation given in the input, find the year of the corresponding Olympiad.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of abbreviations to process. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each containing a single abbreviation. It's guaranteed that each abbreviation contains at most nine digits.</p>

## Output

<p>For each abbreviation given in the input, find the year of the corresponding Olympiad.</p>





```input1
5
IAO'15
IAO'2015
IAO'1
IAO'9
IAO'0

```




```input2
4
IAO'9
IAO'99
IAO'999
IAO'9999

```




```output1
2015
12015
1991
1989
1990

```




```output2
1989
1999
2999
9999

```


