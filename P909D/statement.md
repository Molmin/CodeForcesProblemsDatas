## Description

<div><p>You are given a set of points on a straight line. Each point has a color assigned to it. For point <span class="tex-span"><i>a</i></span>, its neighbors are the points which don't have any other points between them and <span class="tex-span"><i>a</i></span>. Each point has at most two neighbors - one from the left and one from the right.</p><p>You perform a sequence of operations on this set of points. In one operation, you delete all points which have a neighbor point of a different color than the point itself. Points are deleted simultaneously, i.e. first you decide which points have to be deleted and then delete them. After that you can perform the next operation etc. If an operation would not delete any points, you can't perform it.</p><p>How many operations will you need to perform until the next operation does not have any points to delete?</p></div><div class="input-specification"><p>Input contains a single string of lowercase English letters 'a'-'z'. The letters give the points' colors in the order in which they are arranged on the line: the first letter gives the color of the leftmost point, the second gives the color of the second point from the left etc.</p><p>The number of the points is between 1 and <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Output one line containing an integer - the number of operations which can be performed on the given set of points until there are no more points to delete.</p></div>

## Input

<p>Input contains a single string of lowercase English letters 'a'-'z'. The letters give the points' colors in the order in which they are arranged on the line: the first letter gives the color of the leftmost point, the second gives the color of the second point from the left etc.</p><p>The number of the points is between 1 and <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>Output one line containing an integer - the number of operations which can be performed on the given set of points until there are no more points to delete.</p>





```input1
aabb

```




```input2
aabcaa

```




```output1
2

```




```output2
1

```



## Note

<p>In the first test case, the first operation will delete two middle points and leave points "ab", which will be deleted with the second operation. There will be no points left to apply the third operation to.</p><p>In the second test case, the first operation will delete the four points in the middle, leaving points "aa". None of them have neighbors of other colors, so the second operation can't be applied.</p>
