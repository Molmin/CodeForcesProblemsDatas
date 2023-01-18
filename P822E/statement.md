## Description

<div><p>The first semester ended. You know, after the end of the first semester the holidays begin. On holidays Noora decided to return to Vičkopolis. As a modest souvenir for Leha, she brought a sausage of length <span class="tex-span"><i>m</i></span> from Pavlopolis. Everyone knows that any sausage can be represented as a string of lowercase English letters, the length of which is equal to the length of the sausage.</p><p>Leha was very pleased with the gift and immediately ate the sausage. But then he realized that it was a quite tactless act, because the sausage was a souvenir! So the hacker immediately went to the butcher shop. Unfortunately, there was only another sausage of length <span class="tex-span"><i>n</i></span> in the shop. However Leha was not upset and bought this sausage. After coming home, he decided to cut the purchased sausage into several pieces and number the pieces starting from <span class="tex-span">1</span> from left to right. Then he wants to select several pieces and glue them together so that the obtained sausage is equal to the sausage that Noora gave. But the hacker can glue two pieces together only when the number of the left piece is less than the number of the right piece. Besides he knows that if he glues more than <span class="tex-span"><i>x</i></span> pieces, Noora will notice that he has falsified souvenir sausage and will be very upset. Of course Leha doesn’t want to upset the girl. The hacker asks you to find out whether he is able to cut the sausage he bought, and then glue some of the pieces so that Noora doesn't notice anything.</p><p>Formally, you are given two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. The length of the string <span class="tex-span"><i>s</i></span> is <span class="tex-span"><i>n</i></span>, the length of the string <span class="tex-span"><i>t</i></span> is <span class="tex-span"><i>m</i></span>. It is required to select several pairwise non-intersecting substrings from <span class="tex-span"><i>s</i></span>, so that their concatenation in the same order as these substrings appear in <span class="tex-span"><i>s</i></span>, is equal to the string <span class="tex-span"><i>t</i></span>. Denote by <span class="tex-span"><i>f</i>(<i>s</i>, <i>t</i>)</span> the minimal number of substrings to be chosen so that their concatenation is equal to the string <span class="tex-span"><i>t</i></span>. If it is impossible to choose such substrings, then <span class="tex-span"><i>f</i>(<i>s</i>, <i>t</i>) = ∞</span>. Leha really wants to know whether it’s true that <span class="tex-span"><i>f</i>(<i>s</i>, <i>t</i>) ≤ <i>x</i></span>.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — length of sausage bought by Leha, i.e. the length of the string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains string <span class="tex-span"><i>s</i></span> of the length <span class="tex-span"><i>n</i></span> consisting of lowercase English letters.</p><p>The third line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>) — length of sausage bought by Noora, i.e. the length of the string <span class="tex-span"><i>t</i></span>.</p><p>The fourth line contains string <span class="tex-span"><i>t</i></span> of the length <span class="tex-span"><i>m</i></span> consisting of lowercase English letters.</p><p>The fifth line contains single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 30</span>) — the maximum number of pieces of sausage that Leha can glue so that Noora doesn’t notice anything.</p></div><div class="output-specification"><p>In the only line print "<span class="tex-font-style-tt">YES</span>" (without quotes), if Leha is able to succeed in creating new sausage so that Noora doesn't notice anything. Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — length of sausage bought by Leha, i.e. the length of the string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains string <span class="tex-span"><i>s</i></span> of the length <span class="tex-span"><i>n</i></span> consisting of lowercase English letters.</p><p>The third line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>) — length of sausage bought by Noora, i.e. the length of the string <span class="tex-span"><i>t</i></span>.</p><p>The fourth line contains string <span class="tex-span"><i>t</i></span> of the length <span class="tex-span"><i>m</i></span> consisting of lowercase English letters.</p><p>The fifth line contains single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 30</span>) — the maximum number of pieces of sausage that Leha can glue so that Noora doesn’t notice anything.</p>

## Output

<p>In the only line print "<span class="tex-font-style-tt">YES</span>" (without quotes), if Leha is able to succeed in creating new sausage so that Noora doesn't notice anything. Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
9
hloyaygrt
6
loyyrt
3

```




```input2
9
hloyaygrt
6
loyyrt
2

```




```output1
YES

```




```output2
NO

```



## Note

<p>Let's consider the first sample.</p><p>In the optimal answer, Leha should cut the sausage he bought in the following way: <span class="tex-font-style-tt">hloyaygrt = h + loy + a + y + g + rt</span>. Then he numbers received parts from <span class="tex-span">1</span> to <span class="tex-span">6</span>:</p><ul> <li> <span class="tex-font-style-tt">h</span> — number <span class="tex-span">1</span> </li><li> <span class="tex-font-style-tt">loy</span> — number <span class="tex-span">2</span> </li><li> <span class="tex-font-style-tt">a</span> — number <span class="tex-span">3</span> </li><li> <span class="tex-font-style-tt">y</span> — number <span class="tex-span">4</span> </li><li> <span class="tex-font-style-tt">g</span> — number <span class="tex-span">5</span> </li><li> <span class="tex-font-style-tt">rt</span> — number <span class="tex-span">6</span> </li></ul><p>Hereupon the hacker should glue the parts with numbers <span class="tex-span">2</span>, <span class="tex-span">4</span> and <span class="tex-span">6</span> and get sausage <span class="tex-font-style-tt">loyygrt</span> equal to one that is given by Noora. Thus, he will have to glue three pieces. Since <span class="tex-span"><i>x</i> = 3</span> you should print "<span class="tex-font-style-tt">YES</span>" (without quotes).</p><p>In the second sample both sausages coincide with sausages from the first sample. However since <span class="tex-span"><i>x</i> = 2</span> you should print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>
