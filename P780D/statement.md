## Description

<div><p>Innokenty is a president of a new football league in Byteland. The first task he should do is to assign short names to all clubs to be shown on TV next to the score. Of course, the short names should be distinct, and Innokenty wants that all short names consist of <span class="tex-font-style-bf">three letters</span>.</p><p>Each club's full name consist of two words: the team's name and the hometown's name, for example, "<span class="tex-font-style-tt">DINAMO BYTECITY</span>". Innokenty doesn't want to assign strange short names, so he wants to choose such short names for each club that: </p><ol> <li> the short name is the same as three first letters of the team's name, for example, for the mentioned club it is "<span class="tex-font-style-tt">DIN</span>", </li><li> or, the first two letters of the short name should be the same as the first two letters of the team's name, while the third letter is the same as the first letter in the hometown's name. For the mentioned club it is "<span class="tex-font-style-tt">DIB</span>". </li></ol><p>Apart from this, there is a rule that if for some club <span class="tex-span"><i>x</i></span> the second option of short name is chosen, then there should be no club, for which the first option is chosen which is the same as the first option for the club <span class="tex-span"><i>x</i></span>. For example, if the above mentioned club has short name "<span class="tex-font-style-tt">DIB</span>", then no club for which the first option is chosen can have short name equal to "<span class="tex-font-style-tt">DIN</span>". However, it is possible that some club have short name "<span class="tex-font-style-tt">DIN</span>", where "<span class="tex-font-style-tt">DI</span>" are the first two letters of the team's name, and "<span class="tex-font-style-tt">N</span>" is the first letter of hometown's name. Of course, no two teams can have the same short name.</p><p>Help Innokenty to choose a short name for each of the teams. If this is impossible, report that. If there are multiple answer, any of them will suit Innokenty. If for some team the two options of short name are equal, then Innokenty will formally think that only one of these options is chosen. </p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of clubs in the league.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two words&nbsp;— the team's name and the hometown's name for some club. Both team's name and hometown's name consist of uppercase English letters and have length at least <span class="tex-span">3</span> and at most <span class="tex-span">20</span>.</p></div><div class="output-specification"><p>It it is not possible to choose short names and satisfy all constraints, print a single line "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">YES</span>". Then print <span class="tex-span"><i>n</i></span> lines, in each line print the chosen short name for the corresponding club. Print the clubs in the same order as they appeared in input.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of clubs in the league.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two words&nbsp;— the team's name and the hometown's name for some club. Both team's name and hometown's name consist of uppercase English letters and have length at least <span class="tex-span">3</span> and at most <span class="tex-span">20</span>.</p>

## Output

<p>It it is not possible to choose short names and satisfy all constraints, print a single line "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">YES</span>". Then print <span class="tex-span"><i>n</i></span> lines, in each line print the chosen short name for the corresponding club. Print the clubs in the same order as they appeared in input.</p><p>If there are multiple answers, print any of them.</p>





```input1
2
DINAMO BYTECITY
FOOTBALL MOSCOW

```




```input2
2
DINAMO BYTECITY
DINAMO BITECITY

```




```input3
3
PLAYFOOTBALL MOSCOW
PLAYVOLLEYBALL SPB
GOGO TECHNOCUP

```




```input4
3
ABC DEF
ABC EFG
ABD OOO

```




```output1
YES
DIN
FOO

```




```output2
NO

```




```output3
YES
PLM
PLS
GOG

```




```output4
YES
ABD
ABE
ABO

```



## Note

<p>In the first sample Innokenty can choose first option for both clubs.</p><p>In the second example it is not possible to choose short names, because it is not possible that one club has first option, and the other has second option if the first options are equal for both clubs.</p><p>In the third example Innokenty can choose the second options for the first two clubs, and the first option for the third club.</p><p>In the fourth example note that it is possible that the chosen short name for some club <span class="tex-span"><i>x</i></span> is the same as the first option of another club <span class="tex-span"><i>y</i></span> if the first options of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are different.</p>
