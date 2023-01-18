## Description

<div><p>Over time, Alexey's mail box got littered with too many letters. Some of them are read, while others are unread.</p><p>Alexey's mail program can either show a list of all letters or show the content of a single letter. As soon as the program shows the content of an unread letter, it becomes read letter (if the program shows the content of a read letter nothing happens). In one click he can do any of the following operations:</p><ul><li> Move from the list of letters to the content of any single letter.</li><li> Return to the list of letters from single letter viewing mode.</li><li> In single letter viewing mode, move to the next or to the previous letter in the list. You cannot move from the first letter to the previous one or from the last letter to the next one.</li></ul><p>The program cannot delete the letters from the list or rearrange them.</p><p>Alexey wants to read all the unread letters and go watch football. Now he is viewing the list of all letters and for each letter he can see if it is read or unread. What minimum number of operations does Alexey need to perform to read all unread letters?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of letters in the mailbox.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers (zeros and ones) — the state of the letter list. The <span class="tex-span"><i>i</i></span>-th number equals either <span class="tex-span">1</span>, if the <span class="tex-span"><i>i</i></span>-th number is unread, or <span class="tex-span">0</span>, if the <span class="tex-span"><i>i</i></span>-th letter is read.</p></div><div class="output-specification"><p>Print a single number — the minimum number of operations needed to make all the letters read.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of letters in the mailbox.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers (zeros and ones) — the state of the letter list. The <span class="tex-span"><i>i</i></span>-th number equals either <span class="tex-span">1</span>, if the <span class="tex-span"><i>i</i></span>-th number is unread, or <span class="tex-span">0</span>, if the <span class="tex-span"><i>i</i></span>-th letter is read.</p>

## Output

<p>Print a single number — the minimum number of operations needed to make all the letters read.</p>





```input1
5
0 1 0 1 0

```




```input2
5
1 1 0 0 1

```




```input3
2
0 0

```




```output1
3

```




```output2
4

```




```output3
0

```



## Note

<p>In the first sample Alexey needs three operations to cope with the task: open the second letter, move to the third one, move to the fourth one.</p><p>In the second sample the action plan: open the first letter, move to the second letter, return to the list, open the fifth letter.</p><p>In the third sample all letters are already read.</p>
