## Description

<div><p>Heidi the Cow is aghast: cracks in the northern Wall? Zombies gathering outside, forming groups, preparing their assault? This must not happen! Quickly, she fetches her HC<span class="tex-span"><sup class="upper-index">2</sup></span> (Handbook of Crazy Constructions) and looks for the right chapter:</p><p><span class="tex-font-style-it">How to build a wall:</span></p><ol> <li> <span class="tex-font-style-it">Take a set of bricks.</span> </li><li> <span class="tex-font-style-it">Select one of the possible wall designs. Computing the number of possible designs is left as an exercise to the reader.</span> </li><li> <span class="tex-font-style-it">Place bricks on top of each other, according to the chosen design.</span> </li></ol><p>This seems easy enough. But Heidi is a Coding Cow, not a Constructing Cow. Her mind keeps coming back to point 2b. Despite the imminent danger of a zombie onslaught, she wonders just how many possible walls she could build with up to <span class="tex-span"><i>n</i></span> bricks.</p><p>A <span class="tex-font-style-it">wall</span> is a set of wall segments as defined in the easy version. How many different walls can be constructed such that the wall consists of at least <span class="tex-span">1</span> and at most <span class="tex-span"><i>n</i></span> bricks? Two walls are different if there exist a column <span class="tex-span"><i>c</i></span> and a row <span class="tex-span"><i>r</i></span> such that one wall has a brick in this spot, and the other does not.</p><p>Along with <span class="tex-span"><i>n</i></span>, you will be given <span class="tex-span"><i>C</i></span>, the width of the wall (as defined in the easy version). Return the number of different walls modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>C</i></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 500000</span>, <span class="tex-span">1 ≤ <i>C</i> ≤ 200000</span>.</p></div><div class="output-specification"><p>Print the number of different walls that Heidi could build, modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>C</i></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 500000</span>, <span class="tex-span">1 ≤ <i>C</i> ≤ 200000</span>.</p>

## Output

<p>Print the number of different walls that Heidi could build, modulo <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span>.</p>





```input1
5 1

```




```input2
2 2

```




```input3
3 2

```




```input4
11 5

```




```input5
37 63

```




```output1
5

```




```output2
5

```




```output3
9

```




```output4
4367

```




```output5
230574

```



## Note

<p>The number <span class="tex-span">10<sup class="upper-index">6</sup> + 3</span> is prime.</p><p>In the second sample case, the five walls are: </p><pre class="verbatim"><br>            B        B<br>B., .B, BB, B., and .B<br></pre><p>In the third sample case, the nine walls are the five as in the second sample case and in addition the following four: </p><pre class="verbatim"><br>B    B<br>B    B  B        B<br>B., .B, BB, and BB<br></pre>
