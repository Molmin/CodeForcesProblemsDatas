## Description

<div><p>A remote island chain contains <span class="tex-span"><i>n</i></span> islands, labeled <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. Bidirectional bridges connect the islands to form a simple cycle&nbsp;— a bridge connects islands <span class="tex-span">1</span> and <span class="tex-span">2</span>, islands <span class="tex-span">2</span> and <span class="tex-span">3</span>, and so on, and additionally a bridge connects islands <span class="tex-span"><i>n</i></span> and <span class="tex-span">1</span>. The center of each island contains an identical pedestal, and all but one of the islands has a fragile, uniquely colored statue currently held on the pedestal. The remaining island holds only an empty pedestal.</p><p>The islanders want to rearrange the statues in a new order. To do this, they repeat the following process: First, they choose an island directly adjacent to the island containing an empty pedestal. Then, they painstakingly carry the statue on this island across the adjoining bridge and place it on the empty pedestal.</p><p>Determine if it is possible for the islanders to arrange the statues in the desired order.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the total number of islands.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>)&nbsp;— the statue currently placed on the <span class="tex-span"><i>i</i></span>-th island. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the island has no statue. It is guaranteed that the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) — the desired statues of the <span class="tex-span"><i>i</i></span>th island. Once again, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = 0</span> indicates the island desires no statue. It is guaranteed that the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if the rearrangement can be done in the existing network, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the total number of islands.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>)&nbsp;— the statue currently placed on the <span class="tex-span"><i>i</i></span>-th island. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the island has no statue. It is guaranteed that the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) — the desired statues of the <span class="tex-span"><i>i</i></span>th island. Once again, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = 0</span> indicates the island desires no statue. It is guaranteed that the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if the rearrangement can be done in the existing network, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
3
1 0 2
2 0 1

```




```input2
2
1 0
0 1

```




```input3
4
1 2 3 0
0 3 2 1

```




```output1
YES

```




```output2
YES

```




```output3
NO

```



## Note

<p>In the first sample, the islanders can first move statue <span class="tex-span">1</span> from island <span class="tex-span">1</span> to island <span class="tex-span">2</span>, then move statue <span class="tex-span">2</span> from island <span class="tex-span">3</span> to island <span class="tex-span">1</span>, and finally move statue <span class="tex-span">1</span> from island <span class="tex-span">2</span> to island <span class="tex-span">3</span>.</p><p>In the second sample, the islanders can simply move statue <span class="tex-span">1</span> from island <span class="tex-span">1</span> to island <span class="tex-span">2</span>.</p><p>In the third sample, no sequence of movements results in the desired position.</p>
