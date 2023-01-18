## Description

<div><p>You are given two qubits in state <img align="middle" class="tex-formula" src="file://W05KeauG.png" style="max-width: 100.0%;max-height: 100.0%;"> and an integer <span class="tex-span"><i>index</i></span>. Your task is to create one of the <a href="https://en.wikipedia.org/wiki/Bell_state">Bell states</a> on them according to the <span class="tex-span"><i>index</i></span>:</p><ul><li> <img align="middle" class="tex-formula" src="file://f6NQfiN5.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="file://h2EXTkFf.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="file://wfFYs9vd.png" style="max-width: 100.0%;max-height: 100.0%;"></li><li> <img align="middle" class="tex-formula" src="file://KXumhOeJ.png" style="max-width: 100.0%;max-height: 100.0%;"></li></ul></div><div class="input-specification"><p>You have to implement an operation which takes an array of 2 qubits and an integer as an input and has no output. The "output" of your solution is the state in which it left the input qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {<br>    open Microsoft.Quantum.Primitive;<br>    open Microsoft.Quantum.Canon;<br><br>    operation Solve (qs : Qubit[], index : Int) : ()<br>    {<br>        body<br>        {<br>            // your code here<br>        }<br>    }<br>}</pre></div>

## Input

<p>You have to implement an operation which takes an array of 2 qubits and an integer as an input and has no output. The "output" of your solution is the state in which it left the input qubits.</p><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {<br>    open Microsoft.Quantum.Primitive;<br>    open Microsoft.Quantum.Canon;<br><br>    operation Solve (qs : Qubit[], index : Int) : ()<br>    {<br>        body<br>        {<br>            // your code here<br>        }<br>    }<br>}</pre>