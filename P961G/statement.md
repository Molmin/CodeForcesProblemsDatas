## Description

<div><p>You are given a set of <span class="tex-span"><i>n</i></span> elements indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The weight of <span class="tex-span"><i>i</i></span>-th element is <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. The weight of some subset of a given set is denoted as <img align="middle" class="tex-formula" src="file://A4sQEa9Q.png" style="max-width: 100.0%;max-height: 100.0%;">. The weight of some partition <span class="tex-span"><i>R</i></span> of a given set into <span class="tex-span"><i>k</i></span> subsets is <img align="middle" class="tex-formula" src="file://12hY7vkY.png" style="max-width: 100.0%;max-height: 100.0%;"> (recall that a partition of a given set is a set of its subsets such that every element of the given set belongs to exactly one subset in partition).</p><p>Calculate the sum of weights of all partitions of a given set into exactly <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">non-empty</span> subsets, and print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Two partitions are considered different iff there exist two elements <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> such that they belong to the same set in one of the partitions, and to different sets in another partition.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of elements and the number of subsets in each partition, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)— weights of elements of the set.</p></div><div class="output-specification"><p>Print one integer — the sum of weights of all partitions of a given set into <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">non-empty</span> subsets, taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of elements and the number of subsets in each partition, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)— weights of elements of the set.</p>

## Output

<p>Print one integer — the sum of weights of all partitions of a given set into <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">non-empty</span> subsets, taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4 2
2 3 2 3

```




```input2
5 2
1 2 3 4 5

```




```output1
160

```




```output2
645

```



## Note

<p>Possible partitions in the first sample:</p><ol> <li> <span class="tex-span">{{1, 2, 3}, {4}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 3·(<i>w</i><sub class="lower-index">1</sub> + <i>w</i><sub class="lower-index">2</sub> + <i>w</i><sub class="lower-index">3</sub>) + 1·<i>w</i><sub class="lower-index">4</sub> = 24</span>; </li><li> <span class="tex-span">{{1, 2, 4}, {3}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 26</span>; </li><li> <span class="tex-span">{{1, 3, 4}, {2}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 24</span>; </li><li> <span class="tex-span">{{1, 2}, {3, 4}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 2·(<i>w</i><sub class="lower-index">1</sub> + <i>w</i><sub class="lower-index">2</sub>) + 2·(<i>w</i><sub class="lower-index">3</sub> + <i>w</i><sub class="lower-index">4</sub>) = 20</span>; </li><li> <span class="tex-span">{{1, 3}, {2, 4}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 20</span>; </li><li> <span class="tex-span">{{1, 4}, {2, 3}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 20</span>; </li><li> <span class="tex-span">{{1}, {2, 3, 4}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 26</span>; </li></ol><p>Possible partitions in the second sample:</p><ol> <li> <span class="tex-span">{{1, 2, 3, 4}, {5}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 45</span>; </li><li> <span class="tex-span">{{1, 2, 3, 5}, {4}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 48</span>; </li><li> <span class="tex-span">{{1, 2, 4, 5}, {3}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 51</span>; </li><li> <span class="tex-span">{{1, 3, 4, 5}, {2}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 54</span>; </li><li> <span class="tex-span">{{2, 3, 4, 5}, {1}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 57</span>; </li><li> <span class="tex-span">{{1, 2, 3}, {4, 5}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 36</span>; </li><li> <span class="tex-span">{{1, 2, 4}, {3, 5}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 37</span>; </li><li> <span class="tex-span">{{1, 2, 5}, {3, 4}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 38</span>; </li><li> <span class="tex-span">{{1, 3, 4}, {2, 5}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 38</span>; </li><li> <span class="tex-span">{{1, 3, 5}, {2, 4}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 39</span>; </li><li> <span class="tex-span">{{1, 4, 5}, {2, 3}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 40</span>; </li><li> <span class="tex-span">{{2, 3, 4}, {1, 5}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 39</span>; </li><li> <span class="tex-span">{{2, 3, 5}, {1, 4}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 40</span>; </li><li> <span class="tex-span">{{2, 4, 5}, {1, 3}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 41</span>; </li><li> <span class="tex-span">{{3, 4, 5}, {1, 2}}</span>, <span class="tex-span"><i>W</i>(<i>R</i>) = 42</span>. </li></ol>
