## Description

<div><p>Having bought his own apartment, Boris decided to paper the walls in every room. Boris's flat has <span class="tex-span"><i>n</i></span> rooms, each of which has the form of a rectangular parallelepiped. For every room we known its length, width and height of the walls in meters (different rooms can have different dimensions, including height).</p><p>Boris chose <span class="tex-span"><i>m</i></span> types of wallpaper to paper the walls of the rooms with (but it is not necessary to use all the types). Each type of wallpaper is sold in rolls of a fixed length and width (the length, naturally, shows how long the unfolded roll will be). In addition, for each type we know the price of one roll of this type.</p><p>The wallpaper of each type contains strips running along the length of the roll. When gluing the strips must be located strictly vertically (so the roll cannot be rotated, even if the length is less than the width). Besides, a roll can be cut in an arbitrary manner, but the joints of glued pieces should also be vertical. In addition, each room should be papered by only one type of wallpaper. And pieces of the same roll cannot be used to paper different rooms. That is, for each room the rolls are purchased separately. Also, some rolls can be used not completely.</p><p>After buying an apartment Boris is short of cash, so he wants to spend the minimum money on wallpaper. Help him.</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the number of rooms in Boris's apartment.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains three space-separated positive integers — the length, width and height of the walls in a given room in meters, respectively.</p><p>The next line contains a positive integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 500</span>) — the number of available wallpaper types.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains three space-separated positive integers — the length and width in meters of a given wallpaper and the price of one roll, respectively.</p><p>All numbers in the input data do not exceed <span class="tex-span">500</span>. It is guaranteed that each room can be papered using these types of wallpaper.</p></div><div class="output-specification"><p>Print a single number — the minimum total cost of the rolls.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the number of rooms in Boris's apartment.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains three space-separated positive integers — the length, width and height of the walls in a given room in meters, respectively.</p><p>The next line contains a positive integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 500</span>) — the number of available wallpaper types.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains three space-separated positive integers — the length and width in meters of a given wallpaper and the price of one roll, respectively.</p><p>All numbers in the input data do not exceed <span class="tex-span">500</span>. It is guaranteed that each room can be papered using these types of wallpaper.</p>

## Output

<p>Print a single number — the minimum total cost of the rolls.</p>





```input1
1
5 5 3
3
10 1 100
15 2 320
3 19 500

```




```output1
640

```



## Note

<p>Note to the sample:</p><p>The total length of the walls (the perimeter) of the room is 20 m.</p><p>One roll of the first type can be cut into pieces to get three vertical 1 meter wide strips, ergo you need 7 rolls of this type, the price equals 700.</p><p>A roll of the second type can be cut into pieces to get five 2 meter wide strips, we need 2 rolls, the price is 640.</p><p>One roll of the third type can immediately paper 19 meters out of 20, but we cannot use other types and we have to buy a second roll, the price is 1000.</p>
