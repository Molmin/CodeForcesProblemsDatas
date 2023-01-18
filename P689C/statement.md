## Description

<div><p>Bad news came to Mike's village, some thieves stole a bunch of chocolates from the local factory! Horrible! </p><p>Aside from loving sweet things, thieves from this area are known to be very greedy. So after a thief takes his number of chocolates for himself, the next thief will take exactly <span class="tex-span"><i>k</i></span> times more than the previous one. The value of <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> &gt; 1</span>) is a secret integer known only to them. It is also known that each thief's bag can carry at most <span class="tex-span"><i>n</i></span> chocolates (if they intend to take more, the deal is cancelled) and that there were <span class="tex-font-style-bf">exactly four</span> thieves involved. </p><p>Sadly, only the thieves know the value of <span class="tex-span"><i>n</i></span>, but rumours say that the numbers of ways they could have taken the chocolates (for a fixed <span class="tex-span"><i>n</i></span>, but not fixed <span class="tex-span"><i>k</i></span>) is <span class="tex-span"><i>m</i></span>. Two ways are considered different if one of the thieves (they should be numbered in the order they take chocolates) took different number of chocolates in them.</p><p>Mike want to track the thieves down, so he wants to know what their bags are and value of <span class="tex-span"><i>n</i></span> will help him in that. Please find <span class="tex-font-style-bf">the smallest possible</span> value of <span class="tex-span"><i>n</i></span> or tell him that the rumors are false and there is no such <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The single line of input contains the integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">15</sup>)</span>&nbsp;— the number of ways the thieves might steal the chocolates, as rumours say.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>n</i></span>&nbsp;— the maximum amount of chocolates that thieves' bags can carry. If there are more than one <span class="tex-span"><i>n</i></span> satisfying the rumors, <span class="tex-font-style-bf">print the smallest one</span>.</p><p>If there is no such <span class="tex-span"><i>n</i></span> for a false-rumoured <span class="tex-span"><i>m</i></span>, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The single line of input contains the integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">15</sup>)</span>&nbsp;— the number of ways the thieves might steal the chocolates, as rumours say.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>n</i></span>&nbsp;— the maximum amount of chocolates that thieves' bags can carry. If there are more than one <span class="tex-span"><i>n</i></span> satisfying the rumors, <span class="tex-font-style-bf">print the smallest one</span>.</p><p>If there is no such <span class="tex-span"><i>n</i></span> for a false-rumoured <span class="tex-span"><i>m</i></span>, print <span class="tex-span"> - 1</span>.</p>





```input1
1

```




```input2
8

```




```input3
10

```




```output1
8

```




```output2
54

```




```output3
-1

```



## Note

<p>In the first sample case the smallest <span class="tex-span"><i>n</i></span> that leads to exactly one way of stealing chocolates is <span class="tex-span"><i>n</i> = 8</span>, whereas the amounts of stealed chocolates are <span class="tex-span">(1, 2, 4, 8)</span> (the number of chocolates stolen by each of the thieves).</p><p>In the second sample case the smallest <span class="tex-span"><i>n</i></span> that leads to exactly <span class="tex-span">8</span> ways is <span class="tex-span"><i>n</i> = 54</span> with the possibilities: <span class="tex-span">(1, 2, 4, 8),  (1, 3, 9, 27),  (2, 4, 8, 16),  (2, 6, 18, 54),  (3, 6, 12, 24),  (4, 8, 16, 32),  (5, 10, 20, 40),  (6, 12, 24, 48)</span>.</p><p>There is no <span class="tex-span"><i>n</i></span> leading to exactly <span class="tex-span">10</span> ways of stealing chocolates in the third sample case.</p>
