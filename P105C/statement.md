## Description

<div><p>Each item in the game has a level. The higher the level is, the higher basic parameters the item has. We shall consider only the following basic parameters: attack (<span class="tex-font-style-tt">atk</span>), defense (<span class="tex-font-style-tt">def</span>) and resistance to different types of impact (<span class="tex-font-style-tt">res</span>).</p><p>Each item belongs to one class. In this problem we will only consider three of such classes: <span class="tex-font-style-tt">weapon</span>, <span class="tex-font-style-tt">armor</span>, <span class="tex-font-style-tt">orb</span>.</p><p>Besides, there's a whole new world hidden inside each item. We can increase an item's level travelling to its world. We can also capture the so-called residents in the Item World</p><p>Residents are the creatures that live inside items. Each resident gives some bonus to the item in which it is currently located. We will only consider residents of types: <span class="tex-font-style-tt">gladiator</span> (who improves the item's <span class="tex-font-style-tt">atk</span>), <span class="tex-font-style-tt">sentry</span> (who improves <span class="tex-font-style-tt">def</span>) and <span class="tex-font-style-tt">physician</span> (who improves <span class="tex-font-style-tt">res</span>).</p><p>Each item has the size parameter. The parameter limits the maximum number of residents that can live inside an item. We can move residents between items. Within one moment of time we can take some resident from an item and move it to some other item if it has a free place for a new resident. We cannot remove a resident from the items and leave outside — any of them should be inside of some item at any moment of time.</p><p>Laharl has a certain number of items. He wants to move the residents between items so as to equip himself with weapon, armor and a defensive orb. The weapon's <span class="tex-font-style-tt">atk</span> should be largest possible in the end. Among all equipping patterns containing weapon's maximum <span class="tex-font-style-tt">atk</span> parameter we should choose the ones where the armor’s <span class="tex-font-style-tt">def</span> parameter is the largest possible. Among all such equipment patterns we should choose the one where the defensive orb would have the largest possible <span class="tex-font-style-tt">res</span> parameter. Values of the parameters <span class="tex-font-style-tt">def</span> and <span class="tex-font-style-tt">res</span> of weapon, <span class="tex-font-style-tt">atk</span> and <span class="tex-font-style-tt">res</span> of armor and <span class="tex-font-style-tt">atk</span> and <span class="tex-font-style-tt">def</span> of orb are indifferent for Laharl.</p><p>Find the optimal equipment pattern Laharl can get.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — representing how many items Laharl has.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines. Each line contains description of an item. The description has the following form: "<span class="tex-span"><i>name</i></span> <span class="tex-span"><i>class</i></span> <span class="tex-span"><i>atk</i></span> <span class="tex-span"><i>def</i></span> <span class="tex-span"><i>res</i></span> <span class="tex-span"><i>size</i></span>" — the item's name, class, basic attack, defense and resistance parameters and its size correspondingly. </p><ul> <li> <span class="tex-span"><i>name</i></span> and <span class="tex-span"><i>class</i></span> are strings and <span class="tex-span"><i>atk</i></span>, <span class="tex-span"><i>def</i></span>, <span class="tex-span"><i>res</i></span> and <span class="tex-span"><i>size</i></span> are integers. </li><li> <span class="tex-span"><i>name</i></span> consists of lowercase Latin letters and its length can range from <span class="tex-span">1</span> to <span class="tex-span">10</span>, inclusive. </li><li> <span class="tex-span"><i>class</i></span> can be "<span class="tex-font-style-tt">weapon</span>", "<span class="tex-font-style-tt">armor</span>" or "<span class="tex-font-style-tt">orb</span>". </li><li> <span class="tex-span">0 ≤ <i>atk</i>, <i>def</i>, <i>res</i> ≤ 1000</span>. </li><li> <span class="tex-span">1 ≤ <i>size</i> ≤ 10</span>. </li></ul><p>It is guaranteed that Laharl has at least one item of each class.</p><p>The next line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) — the number of residents.</p><p>Then <span class="tex-span"><i>k</i></span> lines follow. Each of them describes a resident. A resident description looks like: "<span class="tex-span"><i>name</i></span> <span class="tex-span"><i>type</i></span> <span class="tex-span"><i>bonus</i></span> <span class="tex-span"><i>home</i></span>" — the resident's name, his type, the number of points the resident adds to the item's corresponding parameter and the name of the item which currently contains the resident. </p><ul> <li> <span class="tex-span"><i>name</i></span>, <span class="tex-span"><i>type</i></span> and <span class="tex-span"><i>home</i></span> are strings and <span class="tex-span"><i>bonus</i></span> is an integer. </li><li> <span class="tex-span"><i>name</i></span> consists of lowercase Latin letters and its length can range from <span class="tex-span">1</span> to <span class="tex-span">10</span>, inclusive. </li><li> <span class="tex-span"><i>type</i></span> may be "<span class="tex-font-style-tt">gladiator</span>", "<span class="tex-font-style-tt">sentry</span>" or "<span class="tex-font-style-tt">physician</span>". </li><li> <span class="tex-span">1 ≤ <i>bonus</i> ≤ 100</span>. </li></ul><p>It is guaranteed that the number of residents in each item does not exceed the item's size.</p><p>The names of all items and residents are pairwise different.</p><p>All words and numbers in the input are separated by single spaces.</p></div><div class="output-specification"><p>Print on the first line the name of the weapon in the optimal equipping pattern; then print the number of residents the weapon contains; then print the residents' names.</p><p>Print on the second and third lines in the same form the names of the armor and defensive orb as well as the residents they contain. </p><p>Use single spaces for separation.</p><p>If there are several possible solutions, print any of them.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — representing how many items Laharl has.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines. Each line contains description of an item. The description has the following form: "<span class="tex-span"><i>name</i></span> <span class="tex-span"><i>class</i></span> <span class="tex-span"><i>atk</i></span> <span class="tex-span"><i>def</i></span> <span class="tex-span"><i>res</i></span> <span class="tex-span"><i>size</i></span>" — the item's name, class, basic attack, defense and resistance parameters and its size correspondingly. </p><ul> <li> <span class="tex-span"><i>name</i></span> and <span class="tex-span"><i>class</i></span> are strings and <span class="tex-span"><i>atk</i></span>, <span class="tex-span"><i>def</i></span>, <span class="tex-span"><i>res</i></span> and <span class="tex-span"><i>size</i></span> are integers. </li><li> <span class="tex-span"><i>name</i></span> consists of lowercase Latin letters and its length can range from <span class="tex-span">1</span> to <span class="tex-span">10</span>, inclusive. </li><li> <span class="tex-span"><i>class</i></span> can be "<span class="tex-font-style-tt">weapon</span>", "<span class="tex-font-style-tt">armor</span>" or "<span class="tex-font-style-tt">orb</span>". </li><li> <span class="tex-span">0 ≤ <i>atk</i>, <i>def</i>, <i>res</i> ≤ 1000</span>. </li><li> <span class="tex-span">1 ≤ <i>size</i> ≤ 10</span>. </li></ul><p>It is guaranteed that Laharl has at least one item of each class.</p><p>The next line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) — the number of residents.</p><p>Then <span class="tex-span"><i>k</i></span> lines follow. Each of them describes a resident. A resident description looks like: "<span class="tex-span"><i>name</i></span> <span class="tex-span"><i>type</i></span> <span class="tex-span"><i>bonus</i></span> <span class="tex-span"><i>home</i></span>" — the resident's name, his type, the number of points the resident adds to the item's corresponding parameter and the name of the item which currently contains the resident. </p><ul> <li> <span class="tex-span"><i>name</i></span>, <span class="tex-span"><i>type</i></span> and <span class="tex-span"><i>home</i></span> are strings and <span class="tex-span"><i>bonus</i></span> is an integer. </li><li> <span class="tex-span"><i>name</i></span> consists of lowercase Latin letters and its length can range from <span class="tex-span">1</span> to <span class="tex-span">10</span>, inclusive. </li><li> <span class="tex-span"><i>type</i></span> may be "<span class="tex-font-style-tt">gladiator</span>", "<span class="tex-font-style-tt">sentry</span>" or "<span class="tex-font-style-tt">physician</span>". </li><li> <span class="tex-span">1 ≤ <i>bonus</i> ≤ 100</span>. </li></ul><p>It is guaranteed that the number of residents in each item does not exceed the item's size.</p><p>The names of all items and residents are pairwise different.</p><p>All words and numbers in the input are separated by single spaces.</p>

## Output

<p>Print on the first line the name of the weapon in the optimal equipping pattern; then print the number of residents the weapon contains; then print the residents' names.</p><p>Print on the second and third lines in the same form the names of the armor and defensive orb as well as the residents they contain. </p><p>Use single spaces for separation.</p><p>If there are several possible solutions, print any of them.</p>





```input1
4
sword weapon 10 2 3 2
pagstarmor armor 0 15 3 1
iceorb orb 3 2 13 2
longbow weapon 9 1 2 1
5
mike gladiator 5 longbow
bobby sentry 6 pagstarmor
petr gladiator 7 iceorb
teddy physician 6 sword
blackjack sentry 8 sword

```




```input2
4
sword weapon 10 2 3 2
pagstarmor armor 0 15 3 1
iceorb orb 3 2 13 2
longbow weapon 9 1 2 1
6
mike gladiator 5 longbow
bobby sentry 6 pagstarmor
petr gladiator 7 iceorb
teddy physician 6 sword
blackjack sentry 8 sword
joe physician 6 iceorb

```




```output1
sword 2 petr mike 
pagstarmor 1 blackjack 
iceorb 2 teddy bobby 

```




```output2
longbow 1 mike 
pagstarmor 1 bobby 
iceorb 2 petr joe 

```



## Note

<p>In the second sample we have no free space inside the items, therefore we cannot move the residents between them.</p>
