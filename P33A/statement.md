## Description

<div><p>In one little known, but very beautiful country called Waterland, lives a lovely shark Valerie. Like all the sharks, she has several rows of teeth, and feeds on crucians. One of Valerie's distinguishing features is that while eating one crucian she uses only one row of her teeth, the rest of the teeth are "relaxing".</p><p>For a long time our heroine had been searching the sea for crucians, but a great misfortune happened. Her teeth started to ache, and she had to see the local dentist, lobster Ashot. As a professional, Ashot quickly relieved Valerie from her toothache. Moreover, he managed to determine the cause of Valerie's developing caries (for what he was later nicknamed Cap).</p><p>It turned that Valerie eats too many crucians. To help Valerie avoid further reoccurrence of toothache, Ashot found for each Valerie's tooth its residual viability. Residual viability of a tooth is a value equal to the amount of crucians that Valerie can eat with this tooth. Every time Valerie eats a crucian, viability of all the teeth used for it will decrease by one. When the viability of at least one tooth becomes negative, the shark will have to see the dentist again. </p><p>Unhappy, Valerie came back home, where a portion of crucians was waiting for her. For sure, the shark couldn't say no to her favourite meal, but she had no desire to go back to the dentist. That's why she decided to eat the maximum amount of crucians from the portion but so that the viability of no tooth becomes negative. </p><p>As Valerie is not good at mathematics, she asked you to help her to find out the total amount of crucians that she can consume for dinner.</p><p>We should remind you that while eating one crucian Valerie uses exactly one row of teeth and the viability of each tooth from this row decreases by one.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 1000, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>) — total amount of Valerie's teeth, amount of tooth rows and amount of crucians in Valerie's portion for dinner. Then follow <span class="tex-span"><i>n</i></span> lines, each containing two integers: <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>m</i></span>) — index of the row, where belongs the corresponding tooth, and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>c</i> ≤ 10<sup class="upper-index">6</sup></span>) — its residual viability.</p><p>It's guaranteed that each tooth row has positive amount of teeth.</p></div><div class="output-specification"><p>In the first line output the maximum amount of crucians that Valerie can consume for dinner.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 1000, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>) — total amount of Valerie's teeth, amount of tooth rows and amount of crucians in Valerie's portion for dinner. Then follow <span class="tex-span"><i>n</i></span> lines, each containing two integers: <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>m</i></span>) — index of the row, where belongs the corresponding tooth, and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>c</i> ≤ 10<sup class="upper-index">6</sup></span>) — its residual viability.</p><p>It's guaranteed that each tooth row has positive amount of teeth.</p>

## Output

<p>In the first line output the maximum amount of crucians that Valerie can consume for dinner.</p>





```input1
4 3 18
2 3
1 2
3 6
2 3

```




```input2
2 2 13
1 13
2 12

```




```output1
11

```




```output2
13

```


