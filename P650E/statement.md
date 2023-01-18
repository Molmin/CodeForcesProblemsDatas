## Description

<div><p>My name is James diGriz, I'm the most clever robber and treasure hunter in the whole galaxy. There are books written about my adventures and songs about my operations, though you were able to catch me up in a pretty awkward moment.</p><p>I was able to hide from cameras, outsmart all the guards and pass numerous traps, but when I finally reached the treasure box and opened it, I have accidentally started the clockwork bomb! Luckily, I have met such kind of bombs before and I know that the clockwork mechanism can be stopped by connecting contacts with wires on the control panel of the bomb in a certain manner.</p><p>I see <span class="tex-span"><i>n</i></span> contacts connected by <span class="tex-span"><i>n</i> - 1</span> wires. Contacts are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Bomb has a security mechanism that ensures the following condition: if there exist <span class="tex-span"><i>k</i> ≥ 2</span> contacts <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span> forming a circuit, i. e. there exist <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">distinct</span> wires between contacts <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">3</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, then the bomb immediately explodes and my story ends here. In particular, if two contacts are connected by more than one wire they form a circuit of length <span class="tex-span">2</span>. It is also prohibited to connect a contact with itself.</p><p>On the other hand, if I disconnect more than one wire (i. e. at some moment there will be no more than <span class="tex-span"><i>n</i> - 2</span> wires in the scheme) then the other security check fails and the bomb also explodes. So, the only thing I can do is to unplug some wire and plug it into a new place ensuring the fact that no circuits appear.</p><p>I know how I should put the wires in order to stop the clockwork. But my time is running out! Help me get out of this alive: find the sequence of operations each of which consists of unplugging some wire and putting it into another place so that the bomb is defused. </p></div><div class="input-specification"><p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500 000</span>), the number of contacts.</p><p>Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains two of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>) denoting the contacts currently connected by the <span class="tex-span"><i>i</i></span>-th wire.</p><p>The remaining <span class="tex-span"><i>n</i> - 1</span> lines contain the description of the sought scheme in the same format.</p><p>It is guaranteed that the starting and the ending schemes are correct (i. e. do not contain cicuits nor wires connecting contact with itself).</p></div><div class="output-specification"><p>The first line should contain <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> ≥ 0</span>)&nbsp;— the minimum number of moves of unplugging and plugging back some wire required to defuse the bomb.</p><p>In each of the following <span class="tex-span"><i>k</i></span> lines output four integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> meaning that on the <span class="tex-span"><i>i</i></span>-th step it is neccesary to unplug the wire connecting the contacts <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and plug it to the contacts <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. Of course the wire connecting contacts <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> should be present in the scheme.</p><p>If there is no correct sequence transforming the existing scheme into the sought one, output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500 000</span>), the number of contacts.</p><p>Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains two of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>) denoting the contacts currently connected by the <span class="tex-span"><i>i</i></span>-th wire.</p><p>The remaining <span class="tex-span"><i>n</i> - 1</span> lines contain the description of the sought scheme in the same format.</p><p>It is guaranteed that the starting and the ending schemes are correct (i. e. do not contain cicuits nor wires connecting contact with itself).</p>

## Output

<p>The first line should contain <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> ≥ 0</span>)&nbsp;— the minimum number of moves of unplugging and plugging back some wire required to defuse the bomb.</p><p>In each of the following <span class="tex-span"><i>k</i></span> lines output four integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> meaning that on the <span class="tex-span"><i>i</i></span>-th step it is neccesary to unplug the wire connecting the contacts <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and plug it to the contacts <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. Of course the wire connecting contacts <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> should be present in the scheme.</p><p>If there is no correct sequence transforming the existing scheme into the sought one, output <span class="tex-font-style-tt">-1</span>.</p>





```input1
3
1 2
2 3
1 3
3 2

```




```input2
4
1 2
2 3
3 4
2 4
4 1
1 3

```




```output1
1
1 2 1 3

```




```output2
3
1 2 1 3
4 3 4 1
2 3 2 4

```



## Note

<p>Picture with the clarification for the sample tests:</p><center> <img class="tex-graphics" height="416px" src="file://Uu36J1Tp.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center>
