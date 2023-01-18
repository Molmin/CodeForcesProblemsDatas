## Description

<div><p>A remote island chain contains <span class="tex-span"><i>n</i></span> islands, with some bidirectional bridges between them. The current bridge network forms a tree. In other words, a total of <span class="tex-span"><i>n</i> - 1</span> bridges connect pairs of islands in a way that it's possible to reach any island from any other island using the bridge network. The center of each island contains an identical pedestal, and all but one of the islands has a fragile, uniquely colored statue currently held on the pedestal. The remaining island holds only an empty pedestal.</p><p>The islanders want to rearrange the statues in a new order. To do this, they repeat the following process: first, they choose an island directly adjacent to the island containing an empty pedestal. Then, they painstakingly carry the statue on this island across the adjoining bridge and place it on the empty pedestal.</p><p>It is often impossible to rearrange statues in the desired order using only the operation described above. The islanders would like to build one additional bridge in order to make this achievable in the fewest number of movements possible. Find the bridge to construct and the minimum number of statue movements necessary to arrange the statues in the desired position.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the total number of islands.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>)&nbsp;— the statue currently located on the <span class="tex-span"><i>i</i></span>-th island. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the island has no statue. It is guaranteed that the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>)&nbsp;— the desired statues of the <span class="tex-span"><i>i</i></span>-th island. Once again, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = 0</span> indicates the island desires no statue. It is guaranteed that the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines each contain two distinct space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the endpoints of the <span class="tex-span"><i>i</i></span>-th bridge. Bridges form a tree, and it is guaranteed that no bridge is listed twice in the input.</p></div><div class="output-specification"><p>Print a single line of integers:</p><p>If the rearrangement can be done in the existing network, output <span class="tex-span">0 <i>t</i></span>, where <span class="tex-span"><i>t</i></span> is the number of moves necessary to perform the rearrangement.</p><p>Otherwise, print <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span>, and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>u</i> &lt; <i>v</i> ≤ <i>n</i></span>)&nbsp;— the two endpoints of the new bridge, and the minimum number of statue movements needed to perform the rearrangement.</p><p>If the rearrangement cannot be done no matter how the new bridge is built, print a single line containing <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the total number of islands.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>)&nbsp;— the statue currently located on the <span class="tex-span"><i>i</i></span>-th island. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the island has no statue. It is guaranteed that the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>)&nbsp;— the desired statues of the <span class="tex-span"><i>i</i></span>-th island. Once again, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = 0</span> indicates the island desires no statue. It is guaranteed that the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines each contain two distinct space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the endpoints of the <span class="tex-span"><i>i</i></span>-th bridge. Bridges form a tree, and it is guaranteed that no bridge is listed twice in the input.</p>

## Output

<p>Print a single line of integers:</p><p>If the rearrangement can be done in the existing network, output <span class="tex-span">0 <i>t</i></span>, where <span class="tex-span"><i>t</i></span> is the number of moves necessary to perform the rearrangement.</p><p>Otherwise, print <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span>, and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>u</i> &lt; <i>v</i> ≤ <i>n</i></span>)&nbsp;— the two endpoints of the new bridge, and the minimum number of statue movements needed to perform the rearrangement.</p><p>If the rearrangement cannot be done no matter how the new bridge is built, print a single line containing <span class="tex-span"> - 1</span>.</p>





```input1
3
1 0 2
2 0 1
1 2
2 3

```




```input2
2
1 0
0 1
1 2

```




```input3
4
0 1 2 3
0 2 3 1
1 2
1 3
1 4

```




```output1
1 3 3

```




```output2
0 1

```




```output3
-1

```



## Note

<p>In the first sample, the islanders can build a bridge connecting islands <span class="tex-span">1</span> and <span class="tex-span">3</span> and then make the following sequence of moves: first move statue <span class="tex-span">1</span> from island <span class="tex-span">1</span> to island <span class="tex-span">2</span>, then move statue <span class="tex-span">2</span> from island <span class="tex-span">3</span> to island <span class="tex-span">1</span>, and finally move statue <span class="tex-span">1</span> from island <span class="tex-span">2</span> to island <span class="tex-span">3</span> for a total of <span class="tex-span">3</span> moves.</p><p>In the second sample, the islanders can simply move statue <span class="tex-span">1</span> from island <span class="tex-span">1</span> to island <span class="tex-span">2</span>. No new bridges need to be built and only <span class="tex-span">1</span> move needs to be made.</p><p>In the third sample, no added bridge and subsequent movements result in the desired position.</p>
