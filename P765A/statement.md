## Description

<div><p>There are literally dozens of snooker competitions held each year, and team Jinotega tries to attend them all (for some reason they prefer name "snookah")! When a competition takes place somewhere far from their hometown, Ivan, Artsem and Konstantin take a flight to the contest and back.</p><p>Jinotega's best friends, team Base have found a list of their itinerary receipts with information about departure and arrival airports. Now they wonder, where is Jinotega now: at home or at some competition far away? They know that: </p><ul> <li> this list contains all Jinotega's flights in this year (<span class="tex-font-style-bf">in arbitrary order</span>), </li><li> Jinotega has only flown from his hometown to a snooker contest and back, </li><li> after each competition Jinotega flies back home (though they may attend a competition in one place several times), </li><li> and finally, at the beginning of the year Jinotega was at home. </li></ul><p>Please help them to determine Jinotega's location!</p></div><div class="input-specification"><p>In the first line of input there is a single integer <span class="tex-span"><i>n</i></span>: the number of Jinotega's flights (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). In the second line there is a string of <span class="tex-span">3</span> capital Latin letters: the name of Jinotega's home airport. In the next <span class="tex-span"><i>n</i></span> lines there is flight information, one flight per line, in form "<span class="tex-font-style-tt">XXX-&gt;YYY</span>", where "<span class="tex-font-style-tt">XXX</span>" is the name of departure airport "<span class="tex-font-style-tt">YYY</span>" is the name of arrival airport. Exactly one of these airports is Jinotega's home airport.</p><p>It is guaranteed that flights information is consistent with the knowledge of Jinotega's friends, which is described in the main part of the statement.</p></div><div class="output-specification"><p>If Jinotega is now at home, print "<span class="tex-font-style-tt">home</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">contest</span>".</p></div>

## Input

<p>In the first line of input there is a single integer <span class="tex-span"><i>n</i></span>: the number of Jinotega's flights (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). In the second line there is a string of <span class="tex-span">3</span> capital Latin letters: the name of Jinotega's home airport. In the next <span class="tex-span"><i>n</i></span> lines there is flight information, one flight per line, in form "<span class="tex-font-style-tt">XXX-&gt;YYY</span>", where "<span class="tex-font-style-tt">XXX</span>" is the name of departure airport "<span class="tex-font-style-tt">YYY</span>" is the name of arrival airport. Exactly one of these airports is Jinotega's home airport.</p><p>It is guaranteed that flights information is consistent with the knowledge of Jinotega's friends, which is described in the main part of the statement.</p>

## Output

<p>If Jinotega is now at home, print "<span class="tex-font-style-tt">home</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">contest</span>".</p>





```input1
4
SVO
SVO-&gt;CDG
LHR-&gt;SVO
SVO-&gt;LHR
CDG-&gt;SVO

```




```input2
3
SVO
SVO-&gt;HKT
HKT-&gt;SVO
SVO-&gt;RAP

```




```output1
home

```




```output2
contest

```



## Note

<p>In the first sample Jinotega might first fly from SVO to CDG and back, and then from SVO to LHR and back, so now they should be at home. In the second sample Jinotega must now be at RAP because a flight from RAP back to SVO is not on the list.</p>
