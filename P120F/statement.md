## Description

<div><p>One day mum asked Petya to sort his toys and get rid of some of them. Petya found a whole box of toy spiders. They were quite dear to him and the boy didn't want to throw them away. Petya conjured a cunning plan: he will glue all the spiders together and attach them to the ceiling. Besides, Petya knows that the lower the spiders will hang, the more mum is going to like it and then she won't throw his favourite toys away. Help Petya carry out the plan.</p><p>A spider consists of <span class="tex-span"><i>k</i></span> beads tied together by <span class="tex-span"><i>k</i> - 1</span> threads. Each thread connects two different beads, at that any pair of beads that make up a spider is either directly connected by a thread, or is connected via some chain of threads and beads.</p><p>Petya may glue spiders together directly gluing their beads. The length of each thread equals 1. The sizes of the beads can be neglected. That's why we can consider that gluing spiders happens by identifying some of the beads (see the picture). Besides, the construction resulting from the gluing process should also represent a spider, that is, it should have the given features. </p><p>After Petya glues all spiders together, he measures the length of the resulting toy. The distance between a pair of beads is identified as the total length of the threads that connect these two beads. The length of the resulting construction is the largest distance between all pairs of beads. Petya wants to make the spider whose length is as much as possible.</p><center> <img class="tex-graphics" height="83px" src="file://iAzRNcLS.png" style="max-width: 100.0%;max-height: 100.0%;" width="249px"> </center><center> <img class="tex-graphics" height="83px" src="file://dOIxarkI.png" style="max-width: 100.0%;max-height: 100.0%;" width="249px"> </center><p>The picture two shows two spiders from the second sample. We can glue to the bead number 2 of the first spider the bead number 1 of the second spider. The threads in the spiders that form the sequence of threads of maximum lengths are highlighted on the picture.</p></div><div class="input-specification"><p>The first input file line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of spiders. Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of each spider: integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of beads, then <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> - 1</span> pairs of numbers denoting the numbers of the beads connected by threads. The beads that make up each spider are numbered from 1 to <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print a single number — the length of the required construction.</p></div>

## Input

<p>The first input file line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of spiders. Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of each spider: integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of beads, then <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> - 1</span> pairs of numbers denoting the numbers of the beads connected by threads. The beads that make up each spider are numbered from 1 to <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print a single number — the length of the required construction.</p>





```input1
1
3 1 2 2 3

```




```input2
2
3 1 2 1 3
4 1 2 2 3 2 4

```




```input3
2
5 1 2 2 3 3 4 3 5
7 3 4 1 2 2 4 4 6 2 7 6 5

```




```output1
2

```




```output2
4

```




```output3
7

```


