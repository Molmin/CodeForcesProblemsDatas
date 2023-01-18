## Description

<div><div class="epigraph"><div class="epigraph-text">For he knew every Who down in Whoville beneath, Was busy now, hanging a mistletoe wreath. "And they're hanging their stockings!" he snarled with a sneer, "Tomorrow is Christmas! It's practically here!"</div><div class="epigraph-source">Dr. Suess, How The Grinch Stole Christmas</div></div><p>Christmas celebrations are coming to Whoville. Cindy Lou Who and her parents Lou Lou Who and Betty Lou Who decided to give sweets to all people in their street. They decided to give the residents of each house on the street, one kilogram of sweets. So they need as many kilos of sweets as there are homes on their street.</p><p>The street, where the Lou Who family lives can be represented as <span class="tex-span"><i>n</i></span> consecutive sections of equal length. You can go from any section to a neighbouring one in one unit of time. Each of the sections is one of three types: an empty piece of land, a house or a shop. Cindy Lou and her family can buy sweets in a shop, but no more than one kilogram of sweets in one shop (the vendors care about the residents of Whoville not to overeat on sweets).</p><p>After the Lou Who family leave their home, they will be on the first section of the road. To get to this section of the road, they also require one unit of time. We can assume that Cindy and her mom and dad can carry an unlimited number of kilograms of sweets. Every time they are on a house section, they can give a kilogram of sweets to the inhabitants of the house, or they can simply move to another section. If the family have already given sweets to the residents of a house, they can't do it again. Similarly, if they are on the shop section, they can either buy a kilo of sweets in it or skip this shop. If they've bought a kilo of sweets in a shop, the seller of the shop remembered them and the won't sell them a single candy if they come again. The time to buy and give sweets can be neglected. The Lou Whos do not want the people of any house to remain without food.</p><p>The Lou Whos want to spend no more than <span class="tex-span"><i>t</i></span> time units of time to give out sweets, as they really want to have enough time to prepare for the Christmas celebration. In order to have time to give all the sweets, they may have to initially bring additional <span class="tex-span"><i>k</i></span> kilos of sweets.</p><p>Cindy Lou wants to know the minimum number of <span class="tex-span"><i>k</i></span> kilos of sweets they need to take with them, to have time to give sweets to the residents of each house in their street.</p><p>Your task is to write a program that will determine the minimum possible value of <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>, 1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line of the input contains <span class="tex-span"><i>n</i></span> characters, the <span class="tex-span"><i>i</i></span>-th of them equals "<span class="tex-font-style-tt">H</span>" (if the <span class="tex-span"><i>i</i></span>-th segment contains a house), "<span class="tex-font-style-tt">S</span>" (if the <span class="tex-span"><i>i</i></span>-th segment contains a shop) or "<span class="tex-font-style-tt">.</span>" (if the <span class="tex-span"><i>i</i></span>-th segment doesn't contain a house or a shop). </p><p>It is guaranteed that there is at least one segment with a house.</p></div><div class="output-specification"><p>If there isn't a single value of <span class="tex-span"><i>k</i></span> that makes it possible to give sweets to everybody in at most <span class="tex-span"><i>t</i></span> units of time, print in a single line "<span class="tex-font-style-tt">-1</span>" (without the quotes). Otherwise, print on a single line the minimum possible value of <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>, 1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line of the input contains <span class="tex-span"><i>n</i></span> characters, the <span class="tex-span"><i>i</i></span>-th of them equals "<span class="tex-font-style-tt">H</span>" (if the <span class="tex-span"><i>i</i></span>-th segment contains a house), "<span class="tex-font-style-tt">S</span>" (if the <span class="tex-span"><i>i</i></span>-th segment contains a shop) or "<span class="tex-font-style-tt">.</span>" (if the <span class="tex-span"><i>i</i></span>-th segment doesn't contain a house or a shop). </p><p>It is guaranteed that there is at least one segment with a house.</p>

## Output

<p>If there isn't a single value of <span class="tex-span"><i>k</i></span> that makes it possible to give sweets to everybody in at most <span class="tex-span"><i>t</i></span> units of time, print in a single line "<span class="tex-font-style-tt">-1</span>" (without the quotes). Otherwise, print on a single line the minimum possible value of <span class="tex-span"><i>k</i></span>.</p>





```input1
6 6
HSHSHS

```




```input2
14 100
...HHHSSS...SH

```




```input3
23 50
HHSS.......SSHHHHHHHHHH

```




```output1
1

```




```output2
0

```




```output3
8

```



## Note

<p>In the first example, there are as many stores, as houses. If the family do not take a single kilo of sweets from home, in order to treat the inhabitants of the first house, they will need to make at least one step back, and they have absolutely no time for it. If they take one kilogram of sweets, they won't need to go back.</p><p>In the second example, the number of shops is equal to the number of houses and plenty of time. Available at all stores passing out candy in one direction and give them when passing in the opposite direction.</p><p>In the third example, the shops on the street are fewer than houses. The Lou Whos have to take the missing number of kilograms of sweets with them from home.</p>
