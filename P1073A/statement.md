## Description

<div><p>You are given a string $s$, consisting of $n$ lowercase Latin letters.</p><p>A substring of string $s$ is a continuous segment of letters from $s$. For example, "<span class="tex-font-style-tt">defor</span>" is a substring of "<span class="tex-font-style-tt">codeforces</span>" and "<span class="tex-font-style-tt">fors</span>" is not. </p><p>The length of the substring is the number of letters in it.</p><p>Let's call some string of length $n$ <span class="tex-font-style-it">diverse</span> if and only if there is no letter to appear strictly more than $\frac n 2$ times. For example, strings "<span class="tex-font-style-tt">abc</span>" and "<span class="tex-font-style-tt">iltlml</span>" are <span class="tex-font-style-it">diverse</span> and strings "<span class="tex-font-style-tt">aab</span>" and "<span class="tex-font-style-tt">zz</span>" are not.</p><p>Your task is to find <span class="tex-font-style-bf">any</span> <span class="tex-font-style-it">diverse</span> substring of string $s$ or report that there is none. Note that it is not required to maximize or minimize the length of the resulting substring.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 1000$) — the length of string $s$.</p><p>The second line is the string $s$, consisting of exactly $n$ lowercase Latin letters.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" if there is no <span class="tex-font-style-it">diverse</span> substring in the string $s$.</p><p>Otherwise the first line should contain "<span class="tex-font-style-tt">YES</span>". The second line should contain <span class="tex-font-style-bf">any</span> <span class="tex-font-style-it">diverse</span> substring of string $s$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 1000$) — the length of string $s$.</p><p>The second line is the string $s$, consisting of exactly $n$ lowercase Latin letters.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" if there is no <span class="tex-font-style-it">diverse</span> substring in the string $s$.</p><p>Otherwise the first line should contain "<span class="tex-font-style-tt">YES</span>". The second line should contain <span class="tex-font-style-bf">any</span> <span class="tex-font-style-it">diverse</span> substring of string $s$.</p>





```input1
10
codeforces

```




```input2
5
aaaaa

```




```output1
YES
code

```




```output2
NO

```



## Note

<p>The first example has lots of correct answers. </p><p>Please, restrain yourself from asking if some specific answer is correct for some specific test or not, these questions always lead to "No comments" answer.</p>
