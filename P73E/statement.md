## Description

<div><p>Vasya plays The Elder Trolls III: Morrowindows. He has a huge list of items in the inventory, however, there is no limits on the size of things. Vasya does not know the total amount of items but he is sure that are not more than <span class="tex-span"><i>x</i></span> and not less than <span class="tex-span">2</span> items in his inventory. A new patch for the game appeared to view inventory in <span class="tex-span"><i>n</i></span> different modes. Displaying in mode <span class="tex-span"><i>i</i></span> is a partition of all inventory items on pages, each of which (except for maybe the last one) shows exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> items. In addition, each mode shows how many pages <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is in a complete list. Great! Perhaps this information will be enough for Vasya to find the required number. Moreover, it is very interesting, what is the fewest number of modes in which Vasya can see inventory to determine the number of items in it?</p><p><span class="tex-font-style-bf">Vasya cannot use the information that was received while looking on inventory in some mode for selection of next actions. I. e. Vasya chooses some set of modes first, and then sees all the results and determines the size.</span></p><p>Knowing the number of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i></span> and assuming that Vasya is very smart, check whether he can uniquely determine the number of items in his inventory, and how many modes he will need to do that if he knows numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i></span> and he is able to know number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> after viewing items in mode <span class="tex-span"><i>i</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 2 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Some numbers among all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> may be equal.</p></div><div class="output-specification"><p>Output the fewest amount of modes required to uniquely determine amount of items in the inventory. If there is no solution output <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 2 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Some numbers among all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> may be equal.</p>

## Output

<p>Output the fewest amount of modes required to uniquely determine amount of items in the inventory. If there is no solution output <span class="tex-span"> - 1</span>.</p>





```input1
2 4
2 3

```




```input2
1 4
2

```




```output1
2

```




```output2
-1

```



## Note

<p>In the second example Vasya is not able to determine items count uniquely because 3 items, as well as 4 items, can be displayed on two pages.</p>
