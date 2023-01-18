## Description

<div><p>Misha hacked the Codeforces site. Then he decided to let all the users change their handles. A user can now change his handle any number of times. But each new handle must not be equal to any handle that is already used or that was used at some point.</p><p>Misha has a list of handle change requests. After completing the requests he wants to understand the relation between the original and the new handles of the users. Help him to do that.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 1000</span>), the number of handle change requests.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain the descriptions of the requests, one per line.</p><p>Each query consists of two non-empty strings <span class="tex-span"><i>old</i></span> and <span class="tex-span"><i>new</i></span>, separated by a space. The strings consist of lowercase and uppercase Latin letters and digits. Strings <span class="tex-span"><i>old</i></span> and <span class="tex-span"><i>new</i></span> are distinct. The lengths of the strings do not exceed <span class="tex-span">20</span>.</p><p>The requests are given chronologically. In other words, by the moment of a query there is a single person with handle <span class="tex-span"><i>old</i></span>, and handle <span class="tex-span"><i>new</i></span> is not used and has not been used by anyone.</p></div><div class="output-specification"><p>In the first line output the integer <span class="tex-span"><i>n</i></span> — the number of users that changed their handles at least once.</p><p>In the next <span class="tex-span"><i>n</i></span> lines print the mapping between the old and the new handles of the users. Each of them must contain two strings, <span class="tex-span"><i>old</i></span> and <span class="tex-span"><i>new</i></span>, separated by a space, meaning that before the user had handle <span class="tex-span"><i>old</i></span>, and after all the requests are completed, his handle is <span class="tex-span"><i>new</i></span>. You may output lines in any order.</p><p>Each user who changes the handle must occur exactly once in this description.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 1000</span>), the number of handle change requests.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain the descriptions of the requests, one per line.</p><p>Each query consists of two non-empty strings <span class="tex-span"><i>old</i></span> and <span class="tex-span"><i>new</i></span>, separated by a space. The strings consist of lowercase and uppercase Latin letters and digits. Strings <span class="tex-span"><i>old</i></span> and <span class="tex-span"><i>new</i></span> are distinct. The lengths of the strings do not exceed <span class="tex-span">20</span>.</p><p>The requests are given chronologically. In other words, by the moment of a query there is a single person with handle <span class="tex-span"><i>old</i></span>, and handle <span class="tex-span"><i>new</i></span> is not used and has not been used by anyone.</p>

## Output

<p>In the first line output the integer <span class="tex-span"><i>n</i></span> — the number of users that changed their handles at least once.</p><p>In the next <span class="tex-span"><i>n</i></span> lines print the mapping between the old and the new handles of the users. Each of them must contain two strings, <span class="tex-span"><i>old</i></span> and <span class="tex-span"><i>new</i></span>, separated by a space, meaning that before the user had handle <span class="tex-span"><i>old</i></span>, and after all the requests are completed, his handle is <span class="tex-span"><i>new</i></span>. You may output lines in any order.</p><p>Each user who changes the handle must occur exactly once in this description.</p>





```input1
5
Misha ILoveCodeforces
Vasya Petrov
Petrov VasyaPetrov123
ILoveCodeforces MikeMirzayanov
Petya Ivanov

```




```output1
3
Petya Ivanov
Misha MikeMirzayanov
Vasya VasyaPetrov123

```


