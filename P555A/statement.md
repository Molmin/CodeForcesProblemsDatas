## Description

<div><p>Andrewid the Android is a galaxy-famous detective. He is now investigating the case of vandalism at the exhibition of contemporary art.</p><p>The main exhibit is a construction of <span class="tex-span"><i>n</i></span> matryoshka dolls that can be nested one into another. The matryoshka dolls are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. A matryoshka with a smaller number can be nested in a matryoshka with a higher number, two matryoshkas can not be directly nested in the same doll, but there may be chain nestings, for example, <span class="tex-span">1 → 2 → 4 → 5</span>. </p><p>In one second, you can perform one of the two following operations:</p><ul> <li> Having a matryoshka <span class="tex-span"><i>a</i></span> that isn't nested in any other matryoshka and a matryoshka <span class="tex-span"><i>b</i></span>, such that <span class="tex-span"><i>b</i></span> doesn't contain any other matryoshka and is not nested in any other matryoshka, you may put <span class="tex-span"><i>a</i></span> in <span class="tex-span"><i>b</i></span>; </li><li> Having a matryoshka <span class="tex-span"><i>a</i></span> directly contained in matryoshka <span class="tex-span"><i>b</i></span>, such that <span class="tex-span"><i>b</i></span> is not nested in any other matryoshka, you may get <span class="tex-span"><i>a</i></span> out of <span class="tex-span"><i>b</i></span>. </li></ul><p>According to the modern aesthetic norms the matryoshka dolls on display were assembled in a specific configuration, i.e. as several separate chains of nested matryoshkas, but the criminal, following the mysterious plan, took out all the dolls and assembled them into a single large chain (<span class="tex-span">1 → 2 → ... → <i>n</i></span>). In order to continue the investigation Andrewid needs to know in what minimum time it is possible to perform this action.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of matryoshkas and matryoshka chains in the initial configuration.</p><p>The next <span class="tex-span"><i>k</i></span> lines contain the descriptions of the chains: the <span class="tex-span"><i>i</i></span>-th line first contains number <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), and then <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>im</i><sub class="lower-index"><i>i</i></sub></sub></span> — the numbers of matryoshkas in the chain (matryoshka <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub></span> is nested into matryoshka <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>2</sub></span>, that is nested into matryoshka <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>3</sub></span>, and so on till the matryoshka <span class="tex-span"><i>a</i><sub class="lower-index"><i>im</i><sub class="lower-index"><i>i</i></sub></sub></span> that isn't nested into any other matryoshka).</p><p>It is guaranteed that <span class="tex-span"><i>m</i><sub class="lower-index">1</sub> + <i>m</i><sub class="lower-index">2</sub> + ... + <i>m</i><sub class="lower-index"><i>k</i></sub> = <i>n</i></span>, the numbers of matryoshkas in all the chains are distinct, in each chain the numbers of matryoshkas follow in the ascending order.</p></div><div class="output-specification"><p>In the single line print the minimum number of seconds needed to assemble one large chain from the initial configuration.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of matryoshkas and matryoshka chains in the initial configuration.</p><p>The next <span class="tex-span"><i>k</i></span> lines contain the descriptions of the chains: the <span class="tex-span"><i>i</i></span>-th line first contains number <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), and then <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>im</i><sub class="lower-index"><i>i</i></sub></sub></span> — the numbers of matryoshkas in the chain (matryoshka <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub></span> is nested into matryoshka <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>2</sub></span>, that is nested into matryoshka <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>3</sub></span>, and so on till the matryoshka <span class="tex-span"><i>a</i><sub class="lower-index"><i>im</i><sub class="lower-index"><i>i</i></sub></sub></span> that isn't nested into any other matryoshka).</p><p>It is guaranteed that <span class="tex-span"><i>m</i><sub class="lower-index">1</sub> + <i>m</i><sub class="lower-index">2</sub> + ... + <i>m</i><sub class="lower-index"><i>k</i></sub> = <i>n</i></span>, the numbers of matryoshkas in all the chains are distinct, in each chain the numbers of matryoshkas follow in the ascending order.</p>

## Output

<p>In the single line print the minimum number of seconds needed to assemble one large chain from the initial configuration.</p>





```input1
3 2
2 1 2
1 3

```




```input2
7 3
3 1 3 7
2 2 5
2 4 6

```




```output1
1

```




```output2
10

```



## Note

<p>In the first sample test there are two chains: <span class="tex-span">1 → 2</span> and <span class="tex-span">3</span>. In one second you can nest the first chain into the second one and get <span class="tex-span">1 → 2 → 3</span>.</p><p>In the second sample test you need to disassemble all the three chains into individual matryoshkas in 2 + 1 + 1 = 4 seconds and then assemble one big chain in 6 seconds.</p>
