## Description

<div><p>One night, having had a hard day at work, Petya saw a nightmare. There was a binary search tree in the dream. But it was not the actual tree that scared Petya. The horrifying thing was that Petya couldn't search for elements in this tree. Petya tried many times to choose key and look for it in the tree, and each time he arrived at a wrong place. Petya has been racking his brains for long, choosing keys many times, but the result was no better. But the moment before Petya would start to despair, he had an epiphany: every time he was looking for keys, the tree didn't have the key, and occured exactly one mistake. "That's not a problem!", thought Petya. "Why not count the expectation value of an element, which is found when I search for the key". The moment he was about to do just that, however, Petya suddenly woke up.</p><p>Thus, you are given a <span class="tex-font-style-underline">binary search tree</span>, that is a tree containing some number written in the node. This number is called the <span class="tex-font-style-underline">node key</span>. The number of children of every node of the tree is equal either to <span class="tex-span">0</span> or to <span class="tex-span">2</span>. The nodes that have <span class="tex-span">0</span> children are called <span class="tex-font-style-underline">leaves</span> and the nodes that have <span class="tex-span">2</span> children, are called <span class="tex-font-style-underline">inner</span>. An inner node has the <span class="tex-font-style-underline">left child</span>, that is the child whose key is less than the current node's key, and the <span class="tex-font-style-underline">right child</span>, whose key is more than the current node's key. Also, a key of any node is strictly larger than all the keys of the left subtree of the node and strictly smaller than all the keys of the right subtree of the node.</p><p>Also you are given a set of <span class="tex-font-style-underline">search keys</span>, all of which are distinct and differ from the node keys contained in the tree. For each key from the set its search in the tree is realised. The search is arranged like this: initially we are located in the tree root, if the key of the current node is larger that our search key, then we move to the left child of the node, otherwise we go to the right child of the node and the process is repeated. As it is guaranteed that the search key is not contained in the tree, the search will always finish in some leaf. The key lying in the leaf is declared the <span class="tex-font-style-underline">search result</span>.</p><p>It is known for sure that during the search we make a mistake in comparing exactly once, that is we go the wrong way, but we won't make any mistakes later. All possible mistakes are equiprobable, that is we should consider all such searches where exactly one mistake occurs. Your task is to find the expectation (the average value) of the search result for every search key, considering that exactly one mistake occurs in the search. That is, for a set of paths containing exactly one mistake in the given key search, you should count the average value of keys containing in the leaves of those paths.</p></div><div class="input-specification"><p>The first line contains an odd integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> &lt; 10<sup class="upper-index">5</sup></span>), which represents the number of tree nodes. Next <span class="tex-span"><i>n</i></span> lines contain node descriptions. The <span class="tex-span">(<i>i</i> + 1)</span>-th line contains two space-separated integers. The first number is the number of parent of the <span class="tex-span"><i>i</i></span>-st node and the second number is the key lying in the <span class="tex-span"><i>i</i></span>-th node. The next line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>), which represents the number of keys for which you should count the average value of search results containing one mistake. Next <span class="tex-span"><i>k</i></span> lines contain the actual keys, one key per line.</p><p>All node keys and all search keys are positive integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>. All <span class="tex-span"><i>n</i> + <i>k</i></span> keys are distinct.</p><p>All nodes are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. For the tree root "-1" (without the quote) will be given instead of the parent's node number. It is guaranteed that the correct binary search tree is given. For each node except for the root, it could be determined according to its key whether it is the left child or the right one.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> real numbers which are the expectations of answers for the keys specified in the input. The answer should differ from the correct one with the measure of absolute or relative error not exceeding <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains an odd integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> &lt; 10<sup class="upper-index">5</sup></span>), which represents the number of tree nodes. Next <span class="tex-span"><i>n</i></span> lines contain node descriptions. The <span class="tex-span">(<i>i</i> + 1)</span>-th line contains two space-separated integers. The first number is the number of parent of the <span class="tex-span"><i>i</i></span>-st node and the second number is the key lying in the <span class="tex-span"><i>i</i></span>-th node. The next line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>), which represents the number of keys for which you should count the average value of search results containing one mistake. Next <span class="tex-span"><i>k</i></span> lines contain the actual keys, one key per line.</p><p>All node keys and all search keys are positive integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>. All <span class="tex-span"><i>n</i> + <i>k</i></span> keys are distinct.</p><p>All nodes are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. For the tree root "-1" (without the quote) will be given instead of the parent's node number. It is guaranteed that the correct binary search tree is given. For each node except for the root, it could be determined according to its key whether it is the left child or the right one.</p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> real numbers which are the expectations of answers for the keys specified in the input. The answer should differ from the correct one with the measure of absolute or relative error not exceeding <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
7
-1 8
1 4
1 12
2 2
2 6
3 10
3 14
1
1

```




```input2
3
-1 5
1 3
1 7
6
1
2
4
6
8
9

```




```output1
8.0000000000

```




```output2
7.0000000000
7.0000000000
7.0000000000
3.0000000000
3.0000000000
3.0000000000

```



## Note

<p>In the first sample the search of key 1 with one error results in two paths in the trees: (1, 2, 5) and (1, 3, 6), in parentheses are listed numbers of nodes from the root to a leaf. The keys in the leaves of those paths are equal to 6 and 10 correspondingly, that's why the answer is equal to 8.</p>
