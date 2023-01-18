## Description

<div><p>You may have heard of the pie rule before. It states that if two people wish to fairly share a slice of pie, one person should cut the slice in half, and the other person should choose who gets which slice. Alice and Bob have many slices of pie, and rather than cutting the slices in half, each individual slice will be eaten by just one person.</p><p>The way Alice and Bob decide who eats each slice is as follows. First, the order in which the pies are to be handed out is decided. There is a special token called the "decider" token, initially held by Bob. Until all the pie is handed out, whoever has the decider token will give the next slice of pie to one of the participants, and the decider token to the other participant. They continue until no slices of pie are left.</p><p>All of the slices are of excellent quality, so each participant obviously wants to maximize the total amount of pie they get to eat. Assuming both players make their decisions optimally, how much pie will each participant receive?</p></div><div class="input-specification"><p>Input will begin with an integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 50</span>), the number of slices of pie. </p><p>Following this is a line with <span class="tex-span"><i>N</i></span> integers indicating the sizes of the slices (each between <span class="tex-span">1</span> and <span class="tex-span">100000</span>, inclusive), in the order in which they must be handed out.</p></div><div class="output-specification"><p>Print two integers. First, the sum of the sizes of slices eaten by Alice, then the sum of the sizes of the slices eaten by Bob, assuming both players make their decisions optimally.</p></div>

## Input

<p>Input will begin with an integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 50</span>), the number of slices of pie. </p><p>Following this is a line with <span class="tex-span"><i>N</i></span> integers indicating the sizes of the slices (each between <span class="tex-span">1</span> and <span class="tex-span">100000</span>, inclusive), in the order in which they must be handed out.</p>

## Output

<p>Print two integers. First, the sum of the sizes of slices eaten by Alice, then the sum of the sizes of the slices eaten by Bob, assuming both players make their decisions optimally.</p>





```input1
3
141 592 653

```




```input2
5
10 21 10 21 10

```




```output1
653 733

```




```output2
31 41

```



## Note

<p>In the first example, Bob takes the size <span class="tex-span">141</span> slice for himself and gives the decider token to Alice. Then Alice gives the size <span class="tex-span">592</span> slice to Bob and keeps the decider token for herself, so that she can then give the size <span class="tex-span">653</span> slice to herself.</p>
