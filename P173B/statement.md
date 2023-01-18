## Description

<div><p>"The Chamber of Secrets has been opened again" — this news has spread all around Hogwarts and some of the students have been petrified due to seeing the basilisk. Dumbledore got fired and now Harry is trying to enter the Chamber of Secrets. These aren't good news for Lord Voldemort. The problem is, he doesn't want anybody to be able to enter the chamber. The Dark Lord is going to be busy sucking life out of Ginny.</p><p>The Chamber of Secrets is an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangular grid in which some of the cells are columns. A light ray (and a basilisk's gaze) passes through the columns without changing its direction. But with some spell we can make a column magic to reflect the light ray (or the gaze) in all four directions when it receives the ray. This is shown in the figure below.</p><center> <img class="tex-graphics" src="file://yQGV3q98.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> The left light ray passes through a regular column, and the right ray — through the magic column. </span> </center><p>The basilisk is located at the right side of the lower right cell of the grid and is looking to the left (in the direction of the lower left cell). According to the legend, anyone who meets a basilisk's gaze directly dies immediately. But if someone meets a basilisk's gaze through a column, this person will get petrified. We know that the door to the Chamber is located on the left side of the upper left corner of the grid and anyone who wants to enter will look in the direction of its movement (in the direction of the upper right cell) from that position.</p><center> <img class="tex-graphics" src="file://iBPrJJcO.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> This figure illustrates the first sample test. </span> </center><p>Given the dimensions of the chamber and the location of regular columns, Lord Voldemort has asked you to find the minimum number of columns that we need to make magic so that anyone who wants to enter the chamber would be petrified or just declare that it's impossible to secure the chamber.</p></div><div class="input-specification"><p>The first line of the input contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters. Each character is either "<span class="tex-font-style-tt">.</span>" or "<span class="tex-font-style-tt">#</span>" and represents one cell of the Chamber grid. It's "<span class="tex-font-style-tt">.</span>" if the corresponding cell is empty and "<span class="tex-font-style-tt">#</span>" if it's a regular column.</p></div><div class="output-specification"><p>Print the minimum number of columns to make magic or -1 if it's impossible to do.</p></div>

## Input

<p>The first line of the input contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters. Each character is either "<span class="tex-font-style-tt">.</span>" or "<span class="tex-font-style-tt">#</span>" and represents one cell of the Chamber grid. It's "<span class="tex-font-style-tt">.</span>" if the corresponding cell is empty and "<span class="tex-font-style-tt">#</span>" if it's a regular column.</p>

## Output

<p>Print the minimum number of columns to make magic or -1 if it's impossible to do.</p>





```input1
3 3
.#.
...
.#.

```




```input2
4 3
##.
...
.#.
.#.

```




```output1
2

```




```output2
2

```



## Note

<p>The figure above shows the first sample test. In the first sample we should make both columns magic. The dragon figure represents the basilisk and the binoculars represent the person who will enter the Chamber of secrets. The black star shows the place where the person will be petrified. Yellow lines represent basilisk gaze moving through columns.</p>
