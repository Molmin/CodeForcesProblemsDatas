## Description

<div><p>One winter evening the Hedgehog was relaxing at home in his cozy armchair and clicking through the TV channels. Stumbled on an issue of «TopShop», the Hedgehog was about to change the channel when all of a sudden he was stopped by an advertisement of a new wondrous invention.</p><p>Actually, a vacuum cleaner was advertised there. It was called Marvellous Vacuum and it doesn't even need a human to operate it while it cleans! The vacuum cleaner can move around the flat on its own: it moves in some direction and if it hits an obstacle there, it automatically chooses a new direction. Sooner or later this vacuum cleaner will travel through all the room and clean it all. Having remembered how much time the Hedgehog spends every time on cleaning (surely, no less than a half of the day), he got eager to buy this wonder.</p><p>However, the Hedgehog quickly understood that the cleaner has at least one weak point: it won't clean well in the room's corners because it often won't able to reach the corner due to its shape. To estimate how serious is this drawback in practice, the Hedgehog asked you to write for him the corresponding program.</p><p>You will be given the cleaner's shape in the top view. We will consider only the cases when the vacuum cleaner is represented as a convex polygon. The room is some infinitely large rectangle. We consider one corner of this room and want to find such a rotation of the vacuum cleaner so that it, being pushed into this corner, will leave the minimum possible area in the corner uncovered.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>N</i></span> which represents the number of vertices of the vacuum cleaner's polygon (<span class="tex-span">3 ≤ <i>N</i> ≤ 4·10<sup class="upper-index">4</sup></span>). Then follow <span class="tex-span"><i>N</i></span> lines each containing two numbers — the coordinates of a vertex of the polygon. All the coordinates are integer and their absolute values do not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>It is guaranteed that the given polygon is nondegenerate and convex (no three points lie on the same line). The polygon vertices are given in a clockwise or counter-clockwise direction.</p></div><div class="output-specification"><p>Print the minimum possible uncovered area. The answer will be accepted if it is within <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> of absolute or relative error from the correct answer.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>N</i></span> which represents the number of vertices of the vacuum cleaner's polygon (<span class="tex-span">3 ≤ <i>N</i> ≤ 4·10<sup class="upper-index">4</sup></span>). Then follow <span class="tex-span"><i>N</i></span> lines each containing two numbers — the coordinates of a vertex of the polygon. All the coordinates are integer and their absolute values do not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>It is guaranteed that the given polygon is nondegenerate and convex (no three points lie on the same line). The polygon vertices are given in a clockwise or counter-clockwise direction.</p>

## Output

<p>Print the minimum possible uncovered area. The answer will be accepted if it is within <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> of absolute or relative error from the correct answer.</p>





```input1
4
0 0
1 0
1 1
0 1

```




```input2
8
1 2
2 1
2 -1
1 -2
-1 -2
-2 -1
-2 1
-1 2

```




```output1
0.00000000000000000000
```




```output2
0.50000000000000000000
```


