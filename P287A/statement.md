## Description

<div><p>In the city of Ultima Thule job applicants are often offered an IQ test. </p><p>The test is as follows: the person gets a piece of squared paper with a <span class="tex-span">4 × 4</span> square painted on it. Some of the square's cells are painted black and others are painted white. Your task is to repaint <span class="tex-font-style-bf">at most one</span> cell the other color so that the picture has a <span class="tex-span">2 × 2</span> square, completely consisting of cells of the same color. If the initial picture already has such a square, the person should just say so and the test will be completed. </p><p>Your task is to write a program that determines whether it is possible to pass the test. You cannot pass the test if either repainting any cell or no action doesn't result in a <span class="tex-span">2 × 2</span> square, consisting of cells of the same color.</p></div><div class="input-specification"><p>Four lines contain four characters each: the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals "<span class="tex-font-style-tt">.</span>" if the cell in the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column of the square is painted white, and "<span class="tex-font-style-tt">#</span>", if the cell is black.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if the test can be passed and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p></div>

## Input

<p>Four lines contain four characters each: the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals "<span class="tex-font-style-tt">.</span>" if the cell in the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column of the square is painted white, and "<span class="tex-font-style-tt">#</span>", if the cell is black.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if the test can be passed and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p>





```input1
####
.#..
####
....

```




```input2
####
....
####
....

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first test sample it is enough to repaint the first cell in the second row. After such repainting the required <span class="tex-span">2 × 2</span> square is on the intersection of the <span class="tex-span">1</span>-st and <span class="tex-span">2</span>-nd row with the <span class="tex-span">1</span>-st and <span class="tex-span">2</span>-nd column.</p>
