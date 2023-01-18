## Description

<div><p>Limak is a grizzly bear. He is big and dreadful. You were chilling in the forest when you suddenly met him. It's very unfortunate for you. He will eat all your cookies unless you can demonstrate your mathematical skills. To test you, Limak is going to give you a puzzle to solve.</p><p>It's a well-known fact that Limak, as every bear, owns a set of numbers. You know some information about the set:</p><ul> <li> The elements of the set are distinct positive integers. </li><li> The number of elements in the set is <span class="tex-span"><i>n</i></span>. The number <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span">5</span>. </li><li> All elements are between <span class="tex-span">1</span> and <span class="tex-span"><i>b</i></span>, inclusive: bears don't know numbers greater than <span class="tex-span"><i>b</i></span>. </li><li> For each <span class="tex-span"><i>r</i></span> in <span class="tex-span">{0, 1, 2, 3, 4}</span>, the set contains exactly <img align="middle" class="tex-formula" src="file://lEZNUhe6.png" style="max-width: 100.0%;max-height: 100.0%;"> elements that give remainder <span class="tex-span"><i>r</i></span> when divided by <span class="tex-span">5</span>. (That is, there are <img align="middle" class="tex-formula" src="file://96qnN1Yb.png" style="max-width: 100.0%;max-height: 100.0%;"> elements divisible by <span class="tex-span">5</span>, <img align="middle" class="tex-formula" src="file://UortdsQn.png" style="max-width: 100.0%;max-height: 100.0%;"> elements of the form <span class="tex-span">5<i>k</i> + 1</span>, <img align="middle" class="tex-formula" src="file://Vz9yxxs4.png" style="max-width: 100.0%;max-height: 100.0%;"> elements of the form <span class="tex-span">5<i>k</i> + 2</span>, and so on.) </li></ul><p>Limak smiles mysteriously and gives you <span class="tex-span"><i>q</i></span> hints about his set. The <span class="tex-span"><i>i</i></span>-th hint is the following sentence: "If you only look at elements that are between <span class="tex-span">1</span> and <span class="tex-span"><i>upTo</i><sub class="lower-index"><i>i</i></sub></span>, inclusive, you will find exactly <span class="tex-span"><i>quantity</i><sub class="lower-index"><i>i</i></sub></span> such elements in my set."</p><p>In a moment Limak will tell you the actual puzzle, but something doesn't seem right... That smile was very strange. You start to think about a possible reason. Maybe Limak cheated you? Or is he a fair grizzly bear?</p><p>Given <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>q</i></span> and hints, check whether Limak can be fair, i.e. there exists at least one set satisfying the given conditions. If it's possible then print ''<span class="tex-font-style-tt">fair</span>". Otherwise, print ''<span class="tex-font-style-tt">unfair</span>".</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ <i>b</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span"><i>n</i></span> divisible by <span class="tex-span">5</span>) — the size of the set, the upper limit for numbers in the set and the number of hints.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the hints. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>upTo</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>quantity</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>upTo</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i></span>, <span class="tex-span">0 ≤ <i>quantity</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print ''<span class="tex-font-style-tt">fair</span>" if there exists at least one set that has all the required properties and matches all the given hints. Otherwise, print ''<span class="tex-font-style-tt">unfair</span>".</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ <i>b</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span"><i>n</i></span> divisible by <span class="tex-span">5</span>) — the size of the set, the upper limit for numbers in the set and the number of hints.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the hints. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>upTo</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>quantity</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>upTo</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i></span>, <span class="tex-span">0 ≤ <i>quantity</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>Print ''<span class="tex-font-style-tt">fair</span>" if there exists at least one set that has all the required properties and matches all the given hints. Otherwise, print ''<span class="tex-font-style-tt">unfair</span>".</p>





```input1
10 20 1
10 10

```




```input2
10 20 3
15 10
5 0
10 5

```




```input3
10 20 2
15 3
20 10

```




```output1
fair

```




```output2
fair

```




```output3
unfair

```



## Note

<p>In the first example there is only one set satisfying all conditions: {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}.</p><p>In the second example also there is only one set satisfying all conditions: {6, 7, 8, 9, 10, 11, 12, 13, 14, 15}.</p><p>Easy to see that there is no set satisfying all conditions from the third example. So Limak lied to you :-(</p>
