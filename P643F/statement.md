## Description

<div><p>There are <span class="tex-span"><i>n</i></span> bears in the inn and <span class="tex-span"><i>p</i></span> places to sleep. Bears will party together for some number of nights (and days).</p><p>Bears love drinking juice. They don't like wine but they can't distinguish it from juice by taste or smell.</p><p>A bear doesn't sleep unless he drinks wine. A bear must go to sleep a few hours after drinking a wine. He will wake up many days after the party is over.</p><p>Radewoosh is the owner of the inn. He wants to put some number of barrels in front of bears. One barrel will contain wine and all other ones will contain juice. Radewoosh will challenge bears to find a barrel with wine.</p><p>Each night, the following happens in this exact order:</p><ol> <li> Each bear must choose a (maybe empty) set of barrels. The same barrel may be chosen by many bears. </li><li> Each bear drinks a glass from each barrel he chose. </li><li> All bears who drink wine go to sleep (exactly those bears who chose a barrel with wine). They will wake up many days after the party is over. If there are not enough places to sleep then bears lose immediately. </li></ol><p>At the end, if it's sure where wine is and there is at least one awake bear then bears win (unless they have lost before because of the number of places to sleep).</p><p>Radewoosh wants to allow bears to win. He considers <span class="tex-span"><i>q</i></span> scenarios. In the <span class="tex-span"><i>i</i></span>-th scenario the party will last for <span class="tex-span"><i>i</i></span> nights. Then, let <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> denote the maximum number of barrels for which bears surely win if they behave optimally. Let's define <img align="middle" class="tex-formula" src="file://eoAnKA75.png" style="max-width: 100.0%;max-height: 100.0%;">. Your task is to find <img align="middle" class="tex-formula" src="file://EtsU9Gmc.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://3UydrM2v.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the exclusive or (also denoted as XOR).</p><p>Note that the same barrel may be chosen by many bears and all of them will go to sleep at once.</p></div><div class="input-specification"><p>The only line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 130</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 2 000 000</span>)&nbsp;— the number of bears, the number of places to sleep and the number of scenarios, respectively.</p></div><div class="output-specification"><p>Print one integer, equal to <img align="middle" class="tex-formula" src="file://N7wIqnDT.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The only line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 130</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 2 000 000</span>)&nbsp;— the number of bears, the number of places to sleep and the number of scenarios, respectively.</p>

## Output

<p>Print one integer, equal to <img align="middle" class="tex-formula" src="file://N7wIqnDT.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
5 1 3

```




```input2
1 100 4

```




```input3
3 2 1

```




```input4
100 100 100

```




```output1
32

```




```output2
4

```




```output3
7

```




```output4
381863924

```



## Note

<p>In the first sample, there are <span class="tex-span">5</span> bears and only <span class="tex-span">1</span> place to sleep. We have <span class="tex-span"><i>R</i><sub class="lower-index">1</sub> = 6, <i>R</i><sub class="lower-index">2</sub> = 11, <i>R</i><sub class="lower-index">3</sub> = 16</span> so the answer is <img align="middle" class="tex-formula" src="file://Rh7ufvmN.png" style="max-width: 100.0%;max-height: 100.0%;">. Let's analyze the optimal strategy for scenario with <span class="tex-span">2</span> days. There are <span class="tex-span"><i>R</i><sub class="lower-index">2</sub> = 11</span> barrels and <span class="tex-span">10</span> of them contain juice.</p><ul> <li> In the first night, the <span class="tex-span"><i>i</i></span>-th bear chooses a barrel <span class="tex-span"><i>i</i></span> only. <ul> <li> If one of the first <span class="tex-span">5</span> barrels contains wine then one bear goes to sleep. Then, bears win because they know where wine is and there is at least one awake bear. </li><li> But let's say none of the first <span class="tex-span">5</span> barrels contains wine. In the second night, the <span class="tex-span"><i>i</i></span>-th bear chooses a barrel <span class="tex-span">5 + <i>i</i></span>. <ul> <li> If one of barrels <span class="tex-span">6 – 10</span> contains wine then one bear goes to sleep. And again, bears win in such a situation. </li><li> If nobody went to sleep then wine is in a barrel <span class="tex-span">11</span>. </li></ul> </li></ul> </li></ul><p>In the second sample, there is only one bear. He should choose an empty set of barrels in each night. Otherwise, he would maybe get wine and bears would lose (because there must be at least one awake bear). So, for any number of days we have <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub> = 1</span>. The answer is <img align="middle" class="tex-formula" src="file://F4pRY14P.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
