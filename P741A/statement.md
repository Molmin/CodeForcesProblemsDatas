## Description

<div><p><span class="tex-font-style-it">As you have noticed, there are lovely girls in Arpa’s land.</span></p><p>People in Arpa's land are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Everyone has exactly one crush, <span class="tex-span"><i>i</i></span>-th person's crush is person with the number <span class="tex-span"><i>crush</i><sub class="lower-index"><i>i</i></sub></span>.</p><center> <img class="tex-graphics" height="222px" src="file://HDl02Q2L.png" style="max-width: 100.0%;max-height: 100.0%;" width="222px"> </center><p>Someday Arpa shouted <span class="tex-font-style-it">Owf</span> loudly from the top of the palace and a funny game started in Arpa's land. The rules are as follows.</p><p>The game consists of rounds. Assume person <span class="tex-span"><i>x</i></span> wants to start a round, he calls <span class="tex-span"><i>crush</i><sub class="lower-index"><i>x</i></sub></span> and says: "<span class="tex-font-style-tt">Oww...wwf</span>" (the letter <span class="tex-font-style-tt">w</span> is repeated <span class="tex-span"><i>t</i></span> times) and cuts off the phone immediately. If <span class="tex-span"><i>t</i> &gt; 1</span> then <span class="tex-span"><i>crush</i><sub class="lower-index"><i>x</i></sub></span> calls <span class="tex-span"><i>crush</i><sub class="lower-index"><i>crush</i><sub class="lower-index"><i>x</i></sub></sub></span> and says: "<span class="tex-font-style-tt">Oww...wwf</span>" (the letter <span class="tex-font-style-tt">w</span> is repeated <span class="tex-span"><i>t</i> - 1</span> times) and cuts off the phone immediately. The round continues until some person receives an "<span class="tex-font-style-tt">Owf</span>" (<span class="tex-span"><i>t</i> = 1</span>). This person is called the <span class="tex-font-style-it">Joon-Joon</span> of the round. There can't be two rounds at the same time.</p><p>Mehrdad has an evil plan to make the game more funny, he wants to find smallest <span class="tex-span"><i>t</i></span> (<span class="tex-span"><i>t</i> ≥ 1</span>) such that for each person <span class="tex-span"><i>x</i></span>, if <span class="tex-span"><i>x</i></span> starts some round and <span class="tex-span"><i>y</i></span> becomes the Joon-Joon of the round, then by starting from <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>x</i></span> would become the Joon-Joon of the round. Find such <span class="tex-span"><i>t</i></span> for Mehrdad if it's possible.</p><p>Some strange fact in Arpa's land is that someone can be himself's crush (i.e. <span class="tex-span"><i>crush</i><sub class="lower-index"><i>i</i></sub> = <i>i</i></span>).</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of people in Arpa's land.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>i</i></span>-th of them is <span class="tex-span"><i>crush</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>crush</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the number of <span class="tex-span"><i>i</i></span>-th person's crush.</p></div><div class="output-specification"><p>If there is no <span class="tex-span"><i>t</i></span> satisfying the condition, print <span class="tex-font-style-tt">-1</span>. Otherwise print such smallest <span class="tex-span"><i>t</i></span>.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of people in Arpa's land.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>i</i></span>-th of them is <span class="tex-span"><i>crush</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>crush</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the number of <span class="tex-span"><i>i</i></span>-th person's crush.</p>

## Output

<p>If there is no <span class="tex-span"><i>t</i></span> satisfying the condition, print <span class="tex-font-style-tt">-1</span>. Otherwise print such smallest <span class="tex-span"><i>t</i></span>.</p>





```input1
4
2 3 1 4

```




```input2
4
4 4 4 4

```




```input3
4
2 1 4 3

```




```output1
3

```




```output2
-1

```




```output3
1

```



## Note

<p>In the first sample suppose <span class="tex-span"><i>t</i> = 3</span>. </p><p>If the first person starts some round:</p><p>The first person calls the second person and says "<span class="tex-font-style-tt">Owwwf</span>", then the second person calls the third person and says "<span class="tex-font-style-tt">Owwf</span>", then the third person calls the first person and says "<span class="tex-font-style-tt">Owf</span>", so the first person becomes Joon-Joon of the round. So the condition is satisfied if <span class="tex-span"><i>x</i></span> is <span class="tex-span">1</span>.</p><p>The process is similar for the second and the third person.</p><p>If the fourth person starts some round:</p><p>The fourth person calls himself and says "<span class="tex-font-style-tt">Owwwf</span>", then he calls himself again and says "<span class="tex-font-style-tt">Owwf</span>", then he calls himself for another time and says "<span class="tex-font-style-tt">Owf</span>", so the fourth person becomes Joon-Joon of the round. So the condition is satisfied when <span class="tex-span"><i>x</i></span> is <span class="tex-span">4</span>.</p><p>In the last example if the first person starts a round, then the second person becomes the Joon-Joon, and vice versa.</p>
