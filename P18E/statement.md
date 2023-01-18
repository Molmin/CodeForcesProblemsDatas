## Description

<div><p>According to a new ISO standard, a flag of every country should have, strangely enough, a chequered field <span class="tex-span"><i>n</i> × <i>m</i></span>, each square should be wholly painted one of 26 colours. The following restrictions are set: </p><ul> <li> In each row at most two different colours can be used. </li><li> No two adjacent squares can be painted the same colour. </li></ul><p>Pay attention, please, that in one column more than two different colours can be used.</p><p>Berland's government took a decision to introduce changes into their country's flag in accordance with the new standard, at the same time they want these changes to be minimal. By the given description of Berland's flag you should find out the minimum amount of squares that need to be painted different colour to make the flag meet the new ISO standard. You are as well to build one of the possible variants of the new Berland's flag.</p></div><div class="input-specification"><p>The first input line contains 2 integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>) — amount of rows and columns in Berland's flag respectively. Then there follows the flag's description: each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters. Each character is a letter from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">z</span>, and it stands for the colour of the corresponding square.</p></div><div class="output-specification"><p>In the first line output the minimum amount of squares that need to be repainted to make the flag meet the new ISO standard. The following <span class="tex-span"><i>n</i></span> lines should contain one of the possible variants of the new flag. Don't forget that the variant of the flag, proposed by you, should be derived from the old flag with the minimum amount of repainted squares. If the answer isn't unique, output any.</p></div>

## Input

<p>The first input line contains 2 integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>) — amount of rows and columns in Berland's flag respectively. Then there follows the flag's description: each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters. Each character is a letter from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">z</span>, and it stands for the colour of the corresponding square.</p>

## Output

<p>In the first line output the minimum amount of squares that need to be repainted to make the flag meet the new ISO standard. The following <span class="tex-span"><i>n</i></span> lines should contain one of the possible variants of the new flag. Don't forget that the variant of the flag, proposed by you, should be derived from the old flag with the minimum amount of repainted squares. If the answer isn't unique, output any.</p>





```input1
3 4
aaaa
bbbb
cccc

```




```input2
3 3
aba
aba
zzz

```




```output1
6
abab
baba
acac

```




```output2
4
aba
bab
zbz

```


