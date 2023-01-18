## Description

<div><p>The Hexadecimal virus loves playing with number sets — intersecting them, uniting them. One beautiful day she was surprised to find out that Scuzzy, her spherical pet cat, united all sets in one and ate the result! Something had to be done quickly and Hexadecimal rushed to the market.</p><p>The market has <span class="tex-span"><i>n</i></span> sets of numbers on sale. The virus wants to buy the following collection of sets: the number of sets in the collection should be exactly the same as the number of numbers in the union of all bought sets. Moreover, Hexadecimal wants to buy the cheapest suitable collection of set.</p><p>Yet nothing's so easy! As Mainframe is a kingdom of pure rivalry markets, we know that the union of any <span class="tex-span"><i>k</i></span> sets contains no less than <span class="tex-span"><i>k</i></span> distinct numbers (for every positive integer <span class="tex-span"><i>k</i></span>).</p><p>Help the virus choose the suitable collection of sets. The collection can be empty.</p></div><div class="input-specification"><p>The first line contains the only number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) — the number of sets available in the market.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the goods: first we are given <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the number of distinct numbers in the <span class="tex-span"><i>i</i></span>-th set, then follow <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> numbers — the set's elements. We know that the set's elements are distinct positive integers and they do not exceed <span class="tex-span"><i>n</i></span>.</p><p>The last line contains <span class="tex-span"><i>n</i></span> integers whose absolute values do not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> — the price of each set.</p></div><div class="output-specification"><p>Print a single number — the minimum price the virus will have to pay for such a collection of <span class="tex-span"><i>k</i></span> sets that union of the collection's sets would have exactly <span class="tex-span"><i>k</i></span> distinct numbers (<img align="middle" class="tex-formula" src="file://wXuYclcI.png" style="max-width: 100.0%;max-height: 100.0%;">).</p></div>

## Input

<p>The first line contains the only number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) — the number of sets available in the market.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the goods: first we are given <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the number of distinct numbers in the <span class="tex-span"><i>i</i></span>-th set, then follow <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> numbers — the set's elements. We know that the set's elements are distinct positive integers and they do not exceed <span class="tex-span"><i>n</i></span>.</p><p>The last line contains <span class="tex-span"><i>n</i></span> integers whose absolute values do not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> — the price of each set.</p>

## Output

<p>Print a single number — the minimum price the virus will have to pay for such a collection of <span class="tex-span"><i>k</i></span> sets that union of the collection's sets would have exactly <span class="tex-span"><i>k</i></span> distinct numbers (<img align="middle" class="tex-formula" src="file://wXuYclcI.png" style="max-width: 100.0%;max-height: 100.0%;">).</p>





```input1
3
1 1
2 2 3
1 3
10 20 -3

```




```input2
5
2 1 2
2 2 3
2 3 4
2 4 5
2 5 1
1 -1 1 -1 1

```




```input3
5
2 1 2
2 2 3
2 3 4
2 4 5
2 5 1
-1 1 -1 1 -1

```




```output1
-3

```




```output2
0

```




```output3
-1

```


