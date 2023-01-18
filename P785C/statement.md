## Description

<div><p>Anton likes to listen to fairy tales, especially when Danik, Anton's best friend, tells them. Right now Danik tells Anton a fairy tale:</p><p>"Once upon a time, there lived an emperor. He was very rich and had much grain. One day he ordered to build a huge barn to put there all his grain. Best builders were building that barn for three days and three nights. But they overlooked and there remained a little hole in the barn, from which every day sparrows came through. Here flew a sparrow, took a grain and flew away..."</p><p>More formally, the following takes place in the fairy tale. At the beginning of the first day the barn with the capacity of <span class="tex-span"><i>n</i></span> grains was full. Then, every day (starting with the first day) the following happens:</p><ul> <li> <span class="tex-span"><i>m</i></span> grains are brought to the barn. If <span class="tex-span"><i>m</i></span> grains doesn't fit to the barn, the barn becomes full and the grains that doesn't fit are brought back (in this problem we can assume that the grains that doesn't fit to the barn are not taken into account). </li><li> Sparrows come and eat grain. In the <span class="tex-span"><i>i</i></span>-th day <span class="tex-span"><i>i</i></span> sparrows come, that is on the first day one sparrow come, on the second day two sparrows come and so on. Every sparrow eats one grain. If the barn is empty, a sparrow eats nothing. </li></ul><p>Anton is tired of listening how Danik describes every sparrow that eats grain from the barn. Anton doesn't know when the fairy tale ends, so he asked you to determine, by the end of which day the barn will become empty for the first time. Help Anton and write a program that will determine the number of that day!</p></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">18</sup>)</span>&nbsp;— the capacity of the barn and the number of grains that are brought every day.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the number of the day when the barn will become empty for the first time. Days are numbered starting with one.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">18</sup>)</span>&nbsp;— the capacity of the barn and the number of grains that are brought every day.</p>

## Output

<p>Output one integer&nbsp;— the number of the day when the barn will become empty for the first time. Days are numbered starting with one.</p>





```input1
5 2

```




```input2
8 1

```




```output1
4

```




```output2
5

```



## Note

<p>In the first sample the capacity of the barn is five grains and two grains are brought every day. The following happens:</p><ul> <li> At the beginning of the first day grain is brought to the barn. It's full, so nothing happens. </li><li> At the end of the first day one sparrow comes and eats one grain, so <span class="tex-span">5 - 1 = 4</span> grains remain. </li><li> At the beginning of the second day two grains are brought. The barn becomes full and one grain doesn't fit to it. </li><li> At the end of the second day two sparrows come. <span class="tex-span">5 - 2 = 3</span> grains remain. </li><li> At the beginning of the third day two grains are brought. The barn becomes full again. </li><li> At the end of the third day three sparrows come and eat grain. <span class="tex-span">5 - 3 = 2</span> grains remain. </li><li> At the beginning of the fourth day grain is brought again. <span class="tex-span">2 + 2 = 4</span> grains remain. </li><li> At the end of the fourth day four sparrows come and eat grain. <span class="tex-span">4 - 4 = 0</span> grains remain. The barn is empty. </li></ul><p>So the answer is <span class="tex-span">4</span>, because by the end of the fourth day the barn becomes empty.</p>
