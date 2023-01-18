## Description

<div><p>A bracketed sequence is called correct (regular) if by inserting "+" and "1" you can get a well-formed mathematical expression from it. For example, sequences "<span class="tex-font-style-tt">(())()</span>", "<span class="tex-font-style-tt">()</span>" and "<span class="tex-font-style-tt">(()(()))</span>" are correct, while "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(()</span>" and "<span class="tex-font-style-tt">(()))(</span>" are not.</p><p>The teacher gave Dmitry's class a very strange task&nbsp;— she asked every student to come up with a sequence of arbitrary length, consisting only of opening and closing brackets. After that all the students took turns naming the sequences they had invented. When Dima's turn came, he suddenly realized that all his classmates got the correct bracketed sequence, and whether he got the correct bracketed sequence, he did not know.</p><p>Dima suspects now that he simply missed the word "correct" in the task statement, so now he wants to save the situation by modifying his sequence slightly. More precisely, he can <span class="tex-font-style-bf">the arbitrary number of times</span> (possibly zero) perform the <span class="tex-font-style-it">reorder</span> operation.</p><p>The reorder operation consists of choosing an arbitrary consecutive subsegment (substring) of the sequence and then reordering all the characters in it in an arbitrary way. Such operation takes $l$ nanoseconds, where $l$ is the length of the subsegment being reordered. It's easy to see that reorder operation doesn't change the number of opening and closing brackets. For example for "<span class="tex-font-style-tt">))((</span>" he can choose the substring "<span class="tex-font-style-tt">)(</span>" and do reorder "<span class="tex-font-style-tt">)()(</span>" (this operation will take $2$ nanoseconds).</p><p>Since Dima will soon have to answer, he wants to make his sequence correct as fast as possible. Help him to do this, or determine that it's impossible.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^6$)&nbsp;— the length of Dima's sequence.</p><p>The second line contains string of length $n$, consisting of characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" only.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of nanoseconds to make the sequence correct or "<span class="tex-font-style-tt">-1</span>" if it is impossible to do so.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^6$)&nbsp;— the length of Dima's sequence.</p><p>The second line contains string of length $n$, consisting of characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" only.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of nanoseconds to make the sequence correct or "<span class="tex-font-style-tt">-1</span>" if it is impossible to do so.</p>





```input1
8
))((())(
```




```input2
3
(()
```




```output1
6
```




```output2
-1
```



## Note

<p>In the first example we can firstly reorder the segment from first to the fourth character, replacing it with "<span class="tex-font-style-tt">()()</span>", the whole sequence will be "<span class="tex-font-style-tt">()()())(</span>". And then reorder the segment from the seventh to eighth character, replacing it with "<span class="tex-font-style-tt">()</span>". In the end the sequence will be "<span class="tex-font-style-tt">()()()()</span>", while the total time spent is $4 + 2 = 6$ nanoseconds.</p>
