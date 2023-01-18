## Description

<div><p>It's New Year's Eve soon, so Ivan decided it's high time he started setting the table. Ivan has bought two cakes and cut them into pieces: the first cake has been cut into <span class="tex-span"><i>a</i></span> pieces, and the second one — into <span class="tex-span"><i>b</i></span> pieces.</p><p>Ivan knows that there will be <span class="tex-span"><i>n</i></span> people at the celebration (including himself), so Ivan has set <span class="tex-span"><i>n</i></span> plates for the cakes. Now he is thinking about how to distribute the cakes between the plates. Ivan wants to do it in such a way that all following conditions are met:</p><ol> <li> Each piece of each cake is put on some plate; </li><li> Each plate contains at least one piece of cake; </li><li> No plate contains pieces of both cakes. </li></ol><p>To make his guests happy, Ivan wants to distribute the cakes in such a way that the minimum number of pieces on the plate is maximized. Formally, Ivan wants to know the maximum possible number <span class="tex-span"><i>x</i></span> such that he can distribute the cakes according to the aforementioned conditions, and each plate will contain at least <span class="tex-span"><i>x</i></span> pieces of cake.</p><p>Help Ivan to calculate this number <span class="tex-span"><i>x</i></span>!</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 100</span>, <span class="tex-span">2 ≤ <i>n</i> ≤ <i>a</i> + <i>b</i></span>) — the number of plates, the number of pieces of the first cake, and the number of pieces of the second cake, respectively.</p></div><div class="output-specification"><p>Print the maximum possible number <span class="tex-span"><i>x</i></span> such that Ivan can distribute the cake in such a way that each plate will contain at least <span class="tex-span"><i>x</i></span> pieces of cake.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 100</span>, <span class="tex-span">2 ≤ <i>n</i> ≤ <i>a</i> + <i>b</i></span>) — the number of plates, the number of pieces of the first cake, and the number of pieces of the second cake, respectively.</p>

## Output

<p>Print the maximum possible number <span class="tex-span"><i>x</i></span> such that Ivan can distribute the cake in such a way that each plate will contain at least <span class="tex-span"><i>x</i></span> pieces of cake.</p>





```input1
5 2 3

```




```input2
4 7 10

```




```output1
1

```




```output2
3

```



## Note

<p>In the first example there is only one way to distribute cakes to plates, all of them will have <span class="tex-span">1</span> cake on it.</p><p>In the second example you can have two plates with <span class="tex-span">3</span> and <span class="tex-span">4</span> pieces of the first cake and two plates both with <span class="tex-span">5</span> pieces of the second cake. Minimal number of pieces is <span class="tex-span">3</span>.</p>
