## Description

<div><p>Recently, Olya received a magical square with the size of $2^n\times 2^n$.</p><p>It seems to her sister that one square is boring. Therefore, she asked Olya to perform <span class="tex-font-style-bf">exactly</span> $k$ <span class="tex-font-style-it">splitting operations</span>.</p><p>A <span class="tex-font-style-it">Splitting operation</span> is an operation during which Olya takes a square with side $a$ and cuts it into 4 equal squares with side $\dfrac{a}{2}$. If the side of the square is equal to $1$, then it is impossible to apply a splitting operation to it (see examples for better understanding).</p><p>Olya is happy to fulfill her sister's request, but she also wants <span class="tex-font-style-it">the condition of Olya's happiness</span> to be satisfied after all operations.</p><p><span class="tex-font-style-it">The condition of Olya's happiness</span> will be satisfied if the following statement is fulfilled:</p><p>Let the length of the side of the lower left square be equal to $a$, then the length of the side of the right upper square should also be equal to $a$. There should also be a path between them that consists only of squares with the side of length $a$. All consecutive squares on a path should have a common side.</p><p>Obviously, as long as we have one square, these conditions are met. So Olya is ready to fulfill her sister's request only under the condition that she is satisfied too. Tell her: is it possible to perform exactly $k$ splitting operations in a certain order so that the condition of Olya's happiness is satisfied? If it is possible, tell also the size of the side of squares of which the path from the lower left square to the upper right one will consist.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^3$)&nbsp;— the number of tests.</p><p>Each of the following $t$ lines contains two integers $n_i$ and $k_i$ ($1 \le n_i \le 10^9, 1 \le k_i \le 10^{18}$)&nbsp;— the description of the $i$-th test, which means that initially Olya's square has size of $2^{n_i}\times 2^{n_i}$ and Olya's sister asks her to do exactly $k_i$ splitting operations.</p></div><div class="output-specification"><p>Print $t$ lines, where in the $i$-th line you should output "<span class="tex-font-style-tt">YES</span>" if it is possible to perform $k_i$ splitting operations in the $i$-th test in such a way that the condition of Olya's happiness is satisfied or print "<span class="tex-font-style-tt">NO</span>" otherwise. If you printed "<span class="tex-font-style-tt">YES</span>", then also print the $log_2$ of the length of the side of the squares through space, along which you can build a path from the lower left square to the upper right one.</p><p>You can output each letter in any case (lower or upper).</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^3$)&nbsp;— the number of tests.</p><p>Each of the following $t$ lines contains two integers $n_i$ and $k_i$ ($1 \le n_i \le 10^9, 1 \le k_i \le 10^{18}$)&nbsp;— the description of the $i$-th test, which means that initially Olya's square has size of $2^{n_i}\times 2^{n_i}$ and Olya's sister asks her to do exactly $k_i$ splitting operations.</p>

## Output

<p>Print $t$ lines, where in the $i$-th line you should output "<span class="tex-font-style-tt">YES</span>" if it is possible to perform $k_i$ splitting operations in the $i$-th test in such a way that the condition of Olya's happiness is satisfied or print "<span class="tex-font-style-tt">NO</span>" otherwise. If you printed "<span class="tex-font-style-tt">YES</span>", then also print the $log_2$ of the length of the side of the squares through space, along which you can build a path from the lower left square to the upper right one.</p><p>You can output each letter in any case (lower or upper).</p><p>If there are multiple answers, print any.</p>





```input1
3
1 1
2 2
2 12
```




```output1
YES 0
YES 1
NO
```



## Note

<p>In each of the illustrations, the pictures are shown in order in which Olya applied the operations. The recently-created squares are highlighted with red.</p><p>In the first test, Olya can apply splitting operations in the following order:</p><center> <img class="tex-graphics" height="170px" src="file://4BxZyq4S.png" style="max-width: 100.0%;max-height: 100.0%;" width="340px"> </center><center> <span class="tex-font-size-small">Olya applies one operation on the only existing square.</span> </center><p>The condition of Olya's happiness will be met, since there is a path of squares of the same size from the lower left square to the upper right one:</p><center> <img class="tex-graphics" height="170px" src="file://zhX1XyZq.png" style="max-width: 100.0%;max-height: 100.0%;" width="170px"> </center><p>The length of the sides of the squares on the path is $1$. $log_2(1) = 0$.</p><p>In the second test, Olya can apply splitting operations in the following order:</p><center> <img class="tex-graphics" height="170px" src="file://6f76V8FB.png" style="max-width: 100.0%;max-height: 100.0%;" width="680px"> </center><center> <span class="tex-font-size-small">Olya applies the first operation on the only existing square. She applies the second one on the right bottom square.</span> </center><p>The condition of Olya's happiness will be met, since there is a path of squares of the same size from the lower left square to the upper right one:</p><center> <img class="tex-graphics" height="170px" src="file://G59KJbpG.png" style="max-width: 100.0%;max-height: 100.0%;" width="170px"> </center><p>The length of the sides of the squares on the path is $2$. $log_2(2) = 1$.</p><p>In the third test, it takes $5$ operations for Olya to make the square look like this:</p><center> <img class="tex-graphics" height="170px" src="file://voctgkoG.png" style="max-width: 100.0%;max-height: 100.0%;" width="170px"> </center><p>Since it requires her to perform $7$ splitting operations, and it is impossible to perform them on squares with side equal to $1$, then Olya cannot do anything more and the answer is "<span class="tex-font-style-tt">NO</span>".</p>
