## Description

<div><p>Roma found a new character in the game "World of Darkraft - 2". In this game the character fights monsters, finds the more and more advanced stuff that lets him fight stronger monsters.</p><p>The character can equip himself with <span class="tex-span"><i>k</i></span> distinct types of items. Power of each item depends on its level (positive integer number). Initially the character has one <span class="tex-span">1</span>-level item of each of the <span class="tex-span"><i>k</i></span> types.</p><p>After the victory over the monster the character finds exactly one new randomly generated item. The generation process looks as follows. Firstly the type of the item is defined; each of the <span class="tex-span"><i>k</i></span> types has the same probability. Then the level of the new item is defined. Let's assume that the level of player's item of the chosen type is equal to <span class="tex-span"><i>t</i></span> at the moment. Level of the new item will be chosen uniformly among integers from segment [<span class="tex-span">1</span>; <span class="tex-span"><i>t</i> + 1</span>].</p><p>From the new item and the current player's item of the same type Roma chooses the best one (i.e. the one with greater level) and equips it (if both of them has the same level Roma choses any). The remaining item is sold for coins. Roma sells an item of level <span class="tex-span"><i>x</i></span> of any type for <span class="tex-span"><i>x</i></span> coins.</p><p>Help Roma determine the expected number of earned coins after the victory over <span class="tex-span"><i>n</i></span> monsters.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Print a real number — expected number of earned coins after victory over <span class="tex-span"><i>n</i></span> monsters. The answer is considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>).</p>

## Output

<p>Print a real number — expected number of earned coins after victory over <span class="tex-span"><i>n</i></span> monsters. The answer is considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
1 3

```




```input2
2 1

```




```input3
10 2

```




```output1
1.0000000000

```




```output2
2.3333333333

```




```output3
15.9380768924

```


