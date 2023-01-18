## Description

<div><p>This winter is so... well, you've got the idea :-) The Nvodsk road system can be represented as <span class="tex-span"><i>n</i></span> junctions connected with <span class="tex-span"><i>n</i> - 1</span> bidirectional roads so that there is a path between any two junctions. The organizers of some event want to choose a place to accommodate the participants (junction <span class="tex-span"><i>v</i></span>), and the place to set up the contests (junction <span class="tex-span"><i>u</i></span>). Besides, at the one hand, they want the participants to walk about the city and see the neighbourhood (that's why the distance between <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> should be no less than <span class="tex-span"><i>l</i></span>). On the other hand, they don't want the participants to freeze (so the distance between <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> should be no more than <span class="tex-span"><i>r</i></span>). Besides, for every street we know its beauty — some integer from <span class="tex-span">0</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>. Your task is to choose the path that fits in the length limits and has the largest average beauty. We shall define the average beauty as a median of sequence of the beauties of all roads along the path.</p><p>We can put it more formally like that: let there be a path with the length <span class="tex-span"><i>k</i></span>. Let <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> be a non-decreasing sequence that contains exactly <span class="tex-span"><i>k</i></span> elements. Each number occurs there exactly the number of times a road with such beauty occurs along on path. We will represent the path median as number <span class="tex-span"><i>a</i><sub class="lower-index">⌊<i>k</i> / 2⌋</sub></span>, assuming that <span class="tex-font-style-bf">indexation starting from zero</span> is used. <span class="tex-span">⌊<i>x</i>⌋</span> — is number <span class="tex-span"><i>х</i></span>, rounded down to the nearest integer.</p><p>For example, if <span class="tex-span"><i>a</i> = {0, 5, 12}</span>, then the median equals to <span class="tex-span">5</span>, and if <span class="tex-span"><i>a</i> = {0, 5, 7, 12}</span>, then the median is number <span class="tex-span">7</span>.</p><p>It is guaranteed that there will be at least one path with the suitable quantity of roads.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain descriptions of roads of the Nvodsk, each line contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — junctions <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are connected with a street whose beauty equals <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print two integers — numbers of the junctions, where to accommodate the participants and set up the contests, correspondingly. If there are multiple optimal variants, print any of them.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain descriptions of roads of the Nvodsk, each line contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — junctions <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are connected with a street whose beauty equals <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print two integers — numbers of the junctions, where to accommodate the participants and set up the contests, correspondingly. If there are multiple optimal variants, print any of them.</p>





```input1
6 3 4
1 2 1
2 3 1
3 4 1
4 5 1
5 6 1

```




```input2
6 3 4
1 2 1
2 3 1
3 4 1
4 5 2
5 6 2

```




```input3
5 1 4
1 2 1
1 3 4
3 4 7
3 5 2

```




```input4
8 3 6
1 2 9
2 3 7
3 4 7
4 5 8
5 8 2
3 6 3
2 7 4

```




```output1
4 1

```




```output2
6 3

```




```output3
4 3

```




```output4
5 1

```



## Note

<p>In the first sample all roads have the same beauty. That means that all paths of the positive length have the same median. Thus, any path with length from <span class="tex-span">3</span> to <span class="tex-span">4</span>, inclusive will be valid for us.</p><p>In the second sample the city looks like that: 1 - 2 - 3 - 4 - 5 - 6. Two last roads are more valuable and we should choose any path that contains both of them and has the suitable length. It is either the path between <span class="tex-span">2</span> and <span class="tex-span">6</span> or the path between <span class="tex-span">3</span> and <span class="tex-span">6</span>.</p>
