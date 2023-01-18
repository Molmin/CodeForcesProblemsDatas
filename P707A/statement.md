## Description

<div><p>Small, but very brave, mouse Brain was not accepted to summer school of young villains. He was upset and decided to postpone his plans of taking over the world, but to become a photographer instead.</p><p>As you may know, the coolest photos are on the film (because you can specify the hashtag #film for such).</p><p>Brain took a lot of colourful pictures on colored and black-and-white film. Then he developed and translated it into a digital form. But now, color and black-and-white photos are in one folder, and to sort them, one needs to spend more than one hour!</p><p>As soon as Brain is a photographer not programmer now, he asks you to help him determine for a <span class="tex-font-style-bf">single</span> photo whether it is colored or black-and-white.</p><p>Photo can be represented as a matrix sized <span class="tex-span"><i>n</i> × <i>m</i></span>, and each element of the matrix stores a symbol indicating corresponding pixel color. There are only <span class="tex-span">6</span> colors: </p><ul> <li> 'C' (cyan)</li><li> 'M' (magenta)</li><li> 'Y' (yellow)</li><li> 'W' (white)</li><li> 'G' (grey)</li><li> 'B' (black) </li></ul><p>The photo is considered black-and-white if it has only white, black and grey pixels in it. If there are any of cyan, magenta or yellow pixels in the photo then it is considered colored.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>)&nbsp;— the number of photo pixel matrix rows and columns respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines describing matrix rows follow. Each of them contains <span class="tex-span"><i>m</i></span> space-separated characters describing colors of pixels in a row. Each character in the line is one of the 'C', 'M', 'Y', 'W', 'G' or 'B'.</p></div><div class="output-specification"><p>Print the "#Black&amp;White" (without quotes), if the photo is black-and-white and "#Color" (without quotes), if it is colored, in the only line.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>)&nbsp;— the number of photo pixel matrix rows and columns respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines describing matrix rows follow. Each of them contains <span class="tex-span"><i>m</i></span> space-separated characters describing colors of pixels in a row. Each character in the line is one of the 'C', 'M', 'Y', 'W', 'G' or 'B'.</p>

## Output

<p>Print the "#Black&amp;White" (without quotes), if the photo is black-and-white and "#Color" (without quotes), if it is colored, in the only line.</p>





```input1
2 2
C M
Y Y

```




```input2
3 2
W W
W W
B B

```




```input3
1 1
W

```




```output1
#Color
```




```output2
#Black&amp;White
```




```output3
#Black&amp;White
```


