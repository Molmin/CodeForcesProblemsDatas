## Description

<div><p>Throughout Igor K.'s life he has had many situations worthy of attention. We remember the story with the virus, the story of his mathematical career and of course, his famous programming achievements. However, one does not always adopt new hobbies, one can quit something as well.</p><p>This time Igor K. got disappointed in one of his hobbies: editing and voicing videos. Moreover, he got disappointed in it so much, that he decided to destroy his secret archive for good. </p><p>Igor K. use Pindows XR operation system which represents files and folders by small icons. At that, <span class="tex-span"><i>m</i></span> icons can fit in a horizontal row in any window.</p><p>Igor K.'s computer contains <span class="tex-span"><i>n</i></span> folders in the D: disk's root catalog. The folders are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order from the left to the right and from top to bottom (see the images). At that the folders with secret videos have numbers from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span> inclusive. Igor K. wants to delete them forever, at that making as few frame selections as possible, and then pressing Shift+Delete exactly once. What is the minimum number of times Igor K. will have to select the folder in order to select folders from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span> and only them? Let us note that if some selected folder is selected repeatedly, then it is deselected. Each selection possesses the shape of some rectangle with sides parallel to the screen's borders.</p></div><div class="input-specification"><p>The only line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>n</i></span>). They are the number of folders in Igor K.'s computer, the width of a window and the numbers of the first and the last folders that need to be deleted.</p></div><div class="output-specification"><p>Print a single number: the least possible number of times Igor K. will have to select the folders using frames to select only the folders with numbers from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span>.</p></div>

## Input

<p>The only line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>n</i></span>). They are the number of folders in Igor K.'s computer, the width of a window and the numbers of the first and the last folders that need to be deleted.</p>

## Output

<p>Print a single number: the least possible number of times Igor K. will have to select the folders using frames to select only the folders with numbers from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span>.</p>





```input1
11 4 3 9

```




```input2
20 5 2 20

```




```output1
3

```




```output2
2

```



## Note

<p>The images below illustrate statement tests.</p><p>The first test:</p><p><img class="tex-graphics" src="file://t8cxlfzs.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In this test we can select folders 3 and 4 with out first selection, folders 5, 6, 7, 8 with our second selection and folder 9 with our third, last selection.</p><p>The second test:</p><p><img class="tex-graphics" src="file://b4mHnEU4.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In this test we can first select all folders in the first row (2, 3, 4, 5), then — all other ones.</p>
