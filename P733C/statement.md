## Description

<div><p>There was an epidemic in Monstropolis and all monsters became sick. To recover, all monsters lined up in queue for an appointment to the only doctor in the city.</p><p>Soon, monsters became hungry and began to eat each other. </p><p>One monster can eat other monster if its weight is <span class="tex-font-style-bf">strictly greater</span> than the weight of the monster being eaten, and they stand in the queue next to each other. Monsters eat each other instantly. There are no monsters which are being eaten at the same moment. After the monster <span class="tex-span"><i>A</i></span> eats the monster <span class="tex-span"><i>B</i></span>, the weight of the monster <span class="tex-span"><i>A</i></span> increases by the weight of the eaten monster <span class="tex-span"><i>B</i></span>. In result of such eating the length of the queue decreases by one, all monsters after the eaten one step forward so that there is no empty places in the queue again. A monster can eat several monsters one after another. Initially there were <span class="tex-span"><i>n</i></span> monsters in the queue, the <span class="tex-span"><i>i</i></span>-th of which had weight <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>For example, if weights are <span class="tex-span">[1, 2, 2, 2, 1, 2]</span> (in order of queue, monsters are numbered from <span class="tex-span">1</span> to <span class="tex-span">6</span> from left to right) then some of the options are:</p><ol> <li> the first monster can't eat the second monster because <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 1</span> is not greater than <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> = 2</span>; </li><li> the second monster can't eat the third monster because <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> = 2</span> is not greater than <span class="tex-span"><i>a</i><sub class="lower-index">3</sub> = 2</span>; </li><li> the second monster can't eat the fifth monster because they are not neighbors; </li><li> the second monster can eat the first monster, the queue will be transformed to <span class="tex-span">[3, 2, 2, 1, 2]</span>. </li></ol><p>After some time, someone said a good joke and all monsters recovered. At that moment there were <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> ≤ <i>n</i></span>) monsters in the queue, the <span class="tex-span"><i>j</i></span>-th of which had weight <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>. Both sequences (<span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>) contain the weights of the monsters in the order from the first to the last.</p><p>You are required to provide one of the possible orders of eating monsters which led to the current queue, or to determine that this could not happen. Assume that the doctor didn't make any appointments while monsters were eating each other.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>)&nbsp;— the number of monsters in the initial queue.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the initial weights of the monsters.</p><p>The third line contains single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of monsters in the queue after the joke. </p><p>The fourth line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 5·10<sup class="upper-index">8</sup></span>)&nbsp;— the weights of the monsters after the joke. </p><p>Monsters are listed in the order from the beginning of the queue to the end.</p></div><div class="output-specification"><p>In case if no actions could lead to the final queue, print "NO" (without quotes) in the only line. </p><p>Otherwise print "YES" (without quotes) in the first line. In the next <span class="tex-span"><i>n</i> - <i>k</i></span> lines print actions in the chronological order. In each line print <span class="tex-span"><i>x</i></span>&nbsp;— the index number of the monster in the current queue which eats and, separated by space, the symbol '<span class="tex-font-style-tt">L</span>' if the monster which stays the <span class="tex-span"><i>x</i></span>-th in the queue eats the monster in front of him, or '<span class="tex-font-style-tt">R</span>' if the monster which stays the <span class="tex-span"><i>x</i></span>-th in the queue eats the monster behind him. After each eating the queue is enumerated again. </p><p>When one monster eats another the queue decreases. If there are several answers, print any of them.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>)&nbsp;— the number of monsters in the initial queue.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the initial weights of the monsters.</p><p>The third line contains single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of monsters in the queue after the joke. </p><p>The fourth line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 5·10<sup class="upper-index">8</sup></span>)&nbsp;— the weights of the monsters after the joke. </p><p>Monsters are listed in the order from the beginning of the queue to the end.</p>

## Output

<p>In case if no actions could lead to the final queue, print "NO" (without quotes) in the only line. </p><p>Otherwise print "YES" (without quotes) in the first line. In the next <span class="tex-span"><i>n</i> - <i>k</i></span> lines print actions in the chronological order. In each line print <span class="tex-span"><i>x</i></span>&nbsp;— the index number of the monster in the current queue which eats and, separated by space, the symbol '<span class="tex-font-style-tt">L</span>' if the monster which stays the <span class="tex-span"><i>x</i></span>-th in the queue eats the monster in front of him, or '<span class="tex-font-style-tt">R</span>' if the monster which stays the <span class="tex-span"><i>x</i></span>-th in the queue eats the monster behind him. After each eating the queue is enumerated again. </p><p>When one monster eats another the queue decreases. If there are several answers, print any of them.</p>





```input1
6
1 2 2 2 1 2
2
5 5

```




```input2
5
1 2 3 4 5
1
15

```




```input3
5
1 1 1 3 3
3
2 1 6

```




```output1
YES
2 L
1 R
4 L
3 L

```




```output2
YES
5 L
4 L
3 L
2 L

```




```output3
NO
```



## Note

<p>In the first example, initially there were <span class="tex-span"><i>n</i> = 6</span> monsters, their weights are <span class="tex-span">[1, 2, 2, 2, 1, 2]</span> (in order of queue from the first monster to the last monster). The final queue should be <span class="tex-span">[5, 5]</span>. The following sequence of eatings leads to the final queue:</p><ul> <li> the second monster eats the monster to the left (i.e. the first monster), queue becomes <span class="tex-span">[3, 2, 2, 1, 2]</span>; </li><li> the first monster (note, it was the second on the previous step) eats the monster to the right (i.e. the second monster), queue becomes <span class="tex-span">[5, 2, 1, 2]</span>; </li><li> the fourth monster eats the mosnter to the left (i.e. the third monster), queue becomes <span class="tex-span">[5, 2, 3]</span>; </li><li> the finally, the third monster eats the monster to the left (i.e. the second monster), queue becomes <span class="tex-span">[5, 5]</span>. </li></ul><p>Note that for each step the output contains numbers of the monsters in their current order in the queue.</p>
