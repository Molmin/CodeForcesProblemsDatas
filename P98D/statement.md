## Description

<div><p>In a far away kingdom is the famous Lio Shan monastery. Gods constructed three diamond pillars on the monastery's lawn long ago. Gods also placed on one pillar <span class="tex-span"><i>n</i></span> golden disks of different diameters (in the order of the diameters' decreasing from the bottom to the top). Besides, gods commanded to carry all the disks from the first pillar to the third one according to the following rules:</p><ul><li> you can carry only one disk in one move;</li><li> you cannot put a larger disk on a smaller one.</li></ul> There was no universal opinion concerning what is to happen after the gods' will is done: some people promised world peace and eternal happiness to everyone, whereas others predicted that the kingdom will face communi… (gee, what am I rambling about?) the Armageddon. However, as everybody knew that it was impossible to solve the problem in less than <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> - 1</span> moves and the lazy Lio Shan monks never even started to solve it, everyone lives peacefully even though the problem was never solved and nobody was afraid of the Armageddon.<p>However, the monastery wasn't doing so well lately and the wise prior Ku Sean Sun had to cut some disks at the edges and use the gold for the greater good. Wouldn't you think that the prior is entitled to have an air conditioning system? Besides, staying in the monastery all year is sooo dull… One has to have a go at something new now and then, go skiing, for example… Ku Sean Sun realize how big a mistake he had made only after a while: after he cut the edges, the diameters of some disks got the same; that means that some moves that used to be impossible to make, were at last possible (why, gods never prohibited to put a disk on a disk of the same diameter). Thus, the possible Armageddon can come earlier than was initially planned by gods. Much earlier. So much earlier, in fact, that Ku Sean Sun won't even have time to ski all he wants or relax under the air conditioner.</p><p>The wise prior could never let that last thing happen and he asked one very old and very wise witch PikiWedia to help him. May be she can determine the least number of moves needed to solve the gods' problem. However, the witch laid out her cards and found no answer for the prior. Then he asked you to help him.</p><p>Can you find the shortest solution of the problem, given the number of disks and their diameters? Keep in mind that it is allowed to place disks of the same diameter one on the other one, however, the order in which the disks are positioned on the third pillar in the end should match the initial order of the disks on the first pillar.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> — the number of disks (<span class="tex-span">1 ≤ <i>n</i> ≤ 20</span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> — the disks' diameters after Ku Sean Sun cut their edges. The diameters are given from the bottom to the top (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 20</span>, besides, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> ≥ <i>d</i><sub class="lower-index"><i>i</i> + 1</sub></span> for any <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>).</p></div><div class="output-specification"><p>Print on the first line number <span class="tex-span"><i>m</i></span> — the smallest number of moves to solve the gods' problem. Print on the next <span class="tex-span"><i>m</i></span> lines the description of moves: two space-separated positive integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> that determine the number of the pillar from which the disk is moved and the number of pillar where the disk is moved, correspondingly (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub></span>). </p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> — the number of disks (<span class="tex-span">1 ≤ <i>n</i> ≤ 20</span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> — the disks' diameters after Ku Sean Sun cut their edges. The diameters are given from the bottom to the top (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 20</span>, besides, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> ≥ <i>d</i><sub class="lower-index"><i>i</i> + 1</sub></span> for any <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>).</p>

## Output

<p>Print on the first line number <span class="tex-span"><i>m</i></span> — the smallest number of moves to solve the gods' problem. Print on the next <span class="tex-span"><i>m</i></span> lines the description of moves: two space-separated positive integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> that determine the number of the pillar from which the disk is moved and the number of pillar where the disk is moved, correspondingly (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub></span>). </p>





```input1
3
3 2 1

```




```input2
3
3 1 1

```




```input3
3
3 3 3

```




```output1
7
1 3
1 2
3 2
1 3
2 1
2 3
1 3

```




```output2
5
1 2
1 2
1 3
2 3
2 3

```




```output3
5
1 2
1 2
1 3
2 3
2 3

```



## Note

<p>Pay attention to the third test demonstrating that the order of disks should remain the same in the end, even despite the disks' same radius. If this condition was not necessary to fulfill, the gods' task could have been solved within a smaller number of moves (three — simply moving the three disks from the first pillar on the third one).</p>
