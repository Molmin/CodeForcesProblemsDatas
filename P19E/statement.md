## Description

<div><p>Once upon a time there lived a good fairy A. One day a fine young man B came to her and asked to predict his future. The fairy looked into her magic ball and said that soon the fine young man will meet the most beautiful princess ever and will marry her. Then she drew on a sheet of paper <span class="tex-span"><i>n</i></span> points and joined some of them with segments, each of the segments starts in some point and ends in some other point. Having drawn that picture, she asked the young man to erase one of the segments from the sheet. Then she tries to colour each point red or blue so, that there is no segment having points of the same colour as its ends. If she manages to do so, the prediction will come true. B wants to meet the most beautiful princess, that's why he asks you to help him. Find all the segments that will help him to meet the princess.</p></div><div class="input-specification"><p>The first input line contains two integer numbers: <span class="tex-span"><i>n</i></span> — amount of the drawn points and <span class="tex-span"><i>m</i></span> — amount of the drawn segments (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>). The following <span class="tex-span"><i>m</i></span> lines contain the descriptions of the segments. Each description contains two different space-separated integer numbers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i>, 1 ≤ <i>u</i> ≤ <i>n</i></span>) — indexes of the points, joined by this segment. No segment is met in the description twice.</p></div><div class="output-specification"><p>In the first line output number <span class="tex-span"><i>k</i></span> — amount of the segments in the answer. In the second line output <span class="tex-span"><i>k</i></span> space-separated numbers — indexes of these segments in ascending order. Each index should be output only once. Segments are numbered from 1 in the input order.</p></div>

## Input

<p>The first input line contains two integer numbers: <span class="tex-span"><i>n</i></span> — amount of the drawn points and <span class="tex-span"><i>m</i></span> — amount of the drawn segments (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>). The following <span class="tex-span"><i>m</i></span> lines contain the descriptions of the segments. Each description contains two different space-separated integer numbers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i>, 1 ≤ <i>u</i> ≤ <i>n</i></span>) — indexes of the points, joined by this segment. No segment is met in the description twice.</p>

## Output

<p>In the first line output number <span class="tex-span"><i>k</i></span> — amount of the segments in the answer. In the second line output <span class="tex-span"><i>k</i></span> space-separated numbers — indexes of these segments in ascending order. Each index should be output only once. Segments are numbered from 1 in the input order.</p>





```input1
4 4
1 2
1 3
2 4
3 4

```




```input2
4 5
1 2
2 3
3 4
4 1
1 3

```




```output1
4
1 2 3 4
```




```output2
1
5
```


