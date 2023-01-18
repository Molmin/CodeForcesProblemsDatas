## Description

<div><p>The Hedgehog recently remembered one of his favorite childhood activities, — solving puzzles, and got into it with new vigor. He would sit day in, day out with his friend buried into thousands of tiny pieces of the picture, looking for the required items one by one.</p><p>Soon the Hedgehog came up with a brilliant idea: instead of buying ready-made puzzles, one can take his own large piece of paper with some picture and cut it into many small rectangular pieces, then mix them and solve the resulting puzzle, trying to piece together the picture. The resulting task is even more challenging than the classic puzzle: now all the fragments have the same rectangular shape, and one can assemble the puzzle only relying on the picture drawn on the pieces.</p><p>All puzzle pieces turn out to be of the same size <span class="tex-span"><i>X</i> × <i>Y</i></span>, because the picture is cut first by horizontal cuts with the pitch of <span class="tex-span"><i>X</i></span>, then with vertical cuts with the pitch of <span class="tex-span"><i>Y</i></span>. If we denote the initial size of the picture as <span class="tex-span"><i>A</i> × <i>B</i></span>, then <span class="tex-span"><i>A</i></span> must be divisible by <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>B</i></span> must be divisible by <span class="tex-span"><i>Y</i></span> (<span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> are integer numbers). </p><p>However, not every such cutting of the picture will result in a <span class="tex-font-style-bf">good</span> puzzle. The Hedgehog finds a puzzle good if no two pieces in it are the same (It is <span class="tex-font-style-bf">allowed to rotate</span> the pieces when comparing them, but it is forbidden to turn them over). </p><p>Your task is to count for a given picture the number of good puzzles that you can make from it, and also to find the puzzle with the minimal piece size.</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> which are the sizes of the picture. They are positive integers not exceeding 20.</p><p>Then follow <span class="tex-span"><i>A</i></span> lines containing <span class="tex-span"><i>B</i></span> symbols each, describing the actual picture. The lines only contain uppercase English letters.</p></div><div class="output-specification"><p>In the first line print the number of possible good puzzles (in other words, the number of pairs <span class="tex-span">(<i>X</i>, <i>Y</i>)</span> such that the puzzle with the corresponding element sizes will be good). This number should always be positive, because the whole picture is a good puzzle itself. </p><p>In the second line print two numbers — the sizes <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> of the smallest possible element among all good puzzles. The comparison is made firstly by the area <span class="tex-span"><i>XY</i></span> of one element and secondly — by the length <span class="tex-span"><i>X</i></span>.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> which are the sizes of the picture. They are positive integers not exceeding 20.</p><p>Then follow <span class="tex-span"><i>A</i></span> lines containing <span class="tex-span"><i>B</i></span> symbols each, describing the actual picture. The lines only contain uppercase English letters.</p>

## Output

<p>In the first line print the number of possible good puzzles (in other words, the number of pairs <span class="tex-span">(<i>X</i>, <i>Y</i>)</span> such that the puzzle with the corresponding element sizes will be good). This number should always be positive, because the whole picture is a good puzzle itself. </p><p>In the second line print two numbers — the sizes <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> of the smallest possible element among all good puzzles. The comparison is made firstly by the area <span class="tex-span"><i>XY</i></span> of one element and secondly — by the length <span class="tex-span"><i>X</i></span>.</p>





```input1
2 4
ABDC
ABDC

```




```input2
2 6
ABCCBA
ABCCBA

```




```output1
3
2 1

```




```output2
1
2 6

```



## Note

<p>The picture in the first sample test has the following good puzzles: <span class="tex-span">(2, 1)</span>, <span class="tex-span">(2, 2)</span>, <span class="tex-span">(2, 4)</span>.</p>
