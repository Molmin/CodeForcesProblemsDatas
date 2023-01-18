## Description

<div><p>Polycarp loves not only to take pictures, but also to show his photos to friends. On his personal website he has recently installed a widget that can display <span class="tex-span"><i>n</i></span> photos with the scroll option. At each moment of time the widget displays exactly one photograph with the option showing the previous/next one. From the first photo, you can switch to the second one or to the <span class="tex-span"><i>n</i></span>-th one, from the second photo you can switch to the third one or to the first one, etc. Thus, navigation is performed in a cycle.</p><p>Polycarp's collection consists of <span class="tex-span"><i>m</i></span> photo albums, the <span class="tex-span"><i>i</i></span>-th album contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> photos. Polycarp wants to choose <span class="tex-span"><i>n</i></span> photos and put them on a new widget. To make watching the photos interesting to the visitors, he is going to post pictures so that no two photos from one album were neighboring (each photo will have exactly two neighbors, the first photo's neighbors are the second and the <span class="tex-span"><i>n</i></span>-th one).</p><p>Help Polycarp compile a photo gallery. Select <span class="tex-span"><i>n</i></span> photos from his collection and put them in such order that no two photos from one album went one after the other.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 40</span>), where <span class="tex-span"><i>n</i></span> is the number of photos on the widget, and <span class="tex-span"><i>m</i></span> is the number of albums. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of photos in the <span class="tex-span"><i>i</i></span>-th album.</p></div><div class="output-specification"><p>Print the single number <span class="tex-font-style-tt">-1</span> if there is no solution. Otherwise, print <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> represents the number of the album of the <span class="tex-span"><i>i</i></span>-th picture in the widget. The albums are numbered from 1 in the order of their appearance in the input. If there are several solutions, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 40</span>), where <span class="tex-span"><i>n</i></span> is the number of photos on the widget, and <span class="tex-span"><i>m</i></span> is the number of albums. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of photos in the <span class="tex-span"><i>i</i></span>-th album.</p>

## Output

<p>Print the single number <span class="tex-font-style-tt">-1</span> if there is no solution. Otherwise, print <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> represents the number of the album of the <span class="tex-span"><i>i</i></span>-th picture in the widget. The albums are numbered from 1 in the order of their appearance in the input. If there are several solutions, print any of them.</p>





```input1
4 3
1 3 5

```




```input2
10 2
5 5

```




```input3
10 3
1 10 3

```




```output1
3 1 3 2

```




```output2
2 1 2 1 2 1 2 1 2 1

```




```output3
-1

```


