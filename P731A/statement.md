## Description

<div><p>Grigoriy, like the hero of one famous comedy film, found a job as a night security guard at the museum. At first night he received <span class="tex-font-style-it">embosser</span> and was to take stock of the whole exposition.</p><p><span class="tex-font-style-it">Embosser</span> is a special devise that allows to "print" the text of a plastic tape. Text is printed sequentially, character by character. The device consists of a wheel with a lowercase English letters written in a circle, static pointer to the current letter and a button that print the chosen letter. At one move it's allowed to rotate the alphabetic wheel one step clockwise or counterclockwise. Initially, static pointer points to letter '<span class="tex-font-style-tt">a</span>'. Other letters are located as shown on the picture:</p><center> <img class="tex-graphics" src="file://XinwFbdr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>After Grigoriy add new item to the base he has to print its name on the plastic tape and attach it to the corresponding exhibit. It's not required to return the wheel to its initial position with pointer on the letter '<span class="tex-font-style-tt">a</span>'.</p><p>Our hero is afraid that some exhibits may become alive and start to attack him, so he wants to print the names as fast as possible. Help him, for the given string find the minimum number of rotations of the wheel required to print it.</p></div><div class="input-specification"><p>The only line of input contains the name of some exhibit&nbsp;— the non-empty string consisting of no more than <span class="tex-span">100</span> characters. It's guaranteed that the string consists of only lowercase English letters.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum number of rotations of the wheel, required to print the name given in the input.</p></div>

## Input

<p>The only line of input contains the name of some exhibit&nbsp;— the non-empty string consisting of no more than <span class="tex-span">100</span> characters. It's guaranteed that the string consists of only lowercase English letters.</p>

## Output

<p>Print one integer&nbsp;— the minimum number of rotations of the wheel, required to print the name given in the input.</p>





```input1
zeus

```




```input2
map

```




```input3
ares

```




```output1
18

```




```output2
35

```




```output3
34

```



## Note

<p>&nbsp;</p><center> <img class="tex-graphics" src="file://lfS7Ab8J.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>To print the string from the first sample it would be optimal to perform the following sequence of rotations: </p><ol> <li> from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>' (<span class="tex-span">1</span> rotation counterclockwise), </li><li> from '<span class="tex-font-style-tt">z</span>' to '<span class="tex-font-style-tt">e</span>' (<span class="tex-span">5</span> clockwise rotations), </li><li> from '<span class="tex-font-style-tt">e</span>' to '<span class="tex-font-style-tt">u</span>' (<span class="tex-span">10</span> rotations counterclockwise), </li><li> from '<span class="tex-font-style-tt">u</span>' to '<span class="tex-font-style-tt">s</span>' (<span class="tex-span">2</span> counterclockwise rotations). </li></ol> In total, <span class="tex-span">1 + 5 + 10 + 2 = 18</span> rotations are required.
