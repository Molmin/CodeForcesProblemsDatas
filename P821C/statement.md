## Description

<div><p>Okabe and Super Hacker Daru are stacking and removing boxes. There are <span class="tex-span"><i>n</i></span> boxes numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Initially there are no boxes on the stack.</p><p>Okabe, being a control freak, gives Daru <span class="tex-span">2<i>n</i></span> commands: <span class="tex-span"><i>n</i></span> of which are to add a box to the top of the stack, and <span class="tex-span"><i>n</i></span> of which are to remove a box from the top of the stack and throw it in the trash. Okabe wants Daru to throw away the boxes in the order from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Of course, this means that it might be impossible for Daru to perform some of Okabe's <span class="tex-font-style-it">remove</span> commands, because the required box is not on the top of the stack.</p><p>That's why Daru can decide to wait until Okabe looks away and then reorder the boxes in the stack in any way he wants. He can do it at any point of time between Okabe's commands, but he can't add or remove boxes while he does it.</p><p>Tell Daru the minimum number of times he needs to reorder the boxes so that he can successfully complete all of Okabe's commands. It is guaranteed that every box is added before it is required to be removed.</p></div><div class="input-specification"><p>The first line of input contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of boxes.</p><p>Each of the next <span class="tex-span">2<i>n</i></span> lines of input starts with a string "<span class="tex-font-style-tt">add</span>" or "<span class="tex-font-style-tt">remove</span>". If the line starts with the "<span class="tex-font-style-tt">add</span>", an integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>) follows, indicating that Daru should add the box with number <span class="tex-span"><i>x</i></span> to the top of the stack. </p><p>It is guaranteed that exactly <span class="tex-span"><i>n</i></span> lines contain "<span class="tex-font-style-tt">add</span>" operations, all the boxes added are distinct, and <span class="tex-span"><i>n</i></span> lines contain "<span class="tex-font-style-tt">remove</span>" operations. It is also guaranteed that a box is always added before it is required to be removed.</p></div><div class="output-specification"><p>Print the minimum number of times Daru needs to reorder the boxes to successfully complete all of Okabe's commands.</p></div>

## Input

<p>The first line of input contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of boxes.</p><p>Each of the next <span class="tex-span">2<i>n</i></span> lines of input starts with a string "<span class="tex-font-style-tt">add</span>" or "<span class="tex-font-style-tt">remove</span>". If the line starts with the "<span class="tex-font-style-tt">add</span>", an integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>) follows, indicating that Daru should add the box with number <span class="tex-span"><i>x</i></span> to the top of the stack. </p><p>It is guaranteed that exactly <span class="tex-span"><i>n</i></span> lines contain "<span class="tex-font-style-tt">add</span>" operations, all the boxes added are distinct, and <span class="tex-span"><i>n</i></span> lines contain "<span class="tex-font-style-tt">remove</span>" operations. It is also guaranteed that a box is always added before it is required to be removed.</p>

## Output

<p>Print the minimum number of times Daru needs to reorder the boxes to successfully complete all of Okabe's commands.</p>





```input1
3
add 1
remove
add 2
add 3
remove
remove

```




```input2
7
add 3
add 2
add 1
remove
add 4
remove
remove
remove
add 6
add 7
add 5
remove
remove
remove

```




```output1
1

```




```output2
2

```



## Note

<p>In the first sample, Daru should reorder the boxes after adding box <span class="tex-span">3</span> to the stack.</p><p>In the second sample, Daru should reorder the boxes after adding box <span class="tex-span">4</span> and box <span class="tex-span">7</span> to the stack.</p>
