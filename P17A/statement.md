## Description

<div><p>Nick is interested in prime numbers. Once he read about <span class="tex-font-style-underline">Goldbach problem</span>. It states that every even integer greater than <span class="tex-span">2</span> can be expressed as the sum of two primes. That got Nick's attention and he decided to invent a problem of his own and call it <span class="tex-font-style-underline">Noldbach problem</span>. Since Nick is interested only in prime numbers, Noldbach problem states that at least <span class="tex-span"><i>k</i></span> prime numbers from <span class="tex-span">2</span> to <span class="tex-span"><i>n</i></span> inclusively can be expressed as the sum of three integer numbers: two neighboring prime numbers and <span class="tex-span">1</span>. For example, <span class="tex-font-style-tt">19</span> = <span class="tex-font-style-tt">7</span> + <span class="tex-font-style-tt">11</span> + <span class="tex-font-style-tt">1</span>, or <span class="tex-font-style-tt">13</span> = <span class="tex-font-style-tt">5</span> + <span class="tex-font-style-tt">7</span> + <span class="tex-font-style-tt">1</span>.</p><p>Two prime numbers are called neighboring if there are no other prime numbers between them.</p><p>You are to help Nick, and find out if he is right or wrong.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>Output <span class="tex-font-style-tt">YES</span> if at least <span class="tex-span"><i>k</i></span> prime numbers from <span class="tex-span">2</span> to <span class="tex-span"><i>n</i></span> inclusively can be expressed as it was described above. Otherwise output <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 1000</span>).</p>

## Output

<p>Output <span class="tex-font-style-tt">YES</span> if at least <span class="tex-span"><i>k</i></span> prime numbers from <span class="tex-span">2</span> to <span class="tex-span"><i>n</i></span> inclusively can be expressed as it was described above. Otherwise output <span class="tex-font-style-tt">NO</span>.</p>





```input1
27 2

```




```input2
45 7

```




```output1
YES
```




```output2
NO
```



## Note

<p>In the first sample the answer is <span class="tex-font-style-tt">YES</span> since at least two numbers can be expressed as it was described (for example, 13 and 19). In the second sample the answer is <span class="tex-font-style-tt">NO</span> since it is impossible to express 7 prime numbers from 2 to 45 in the desired form.</p>
