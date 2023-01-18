## Description

<div><p>Vasya writes his own library for building graphical user interface. Vasya called his creation <span class="tex-font-style-tt">VTK</span> (<span class="tex-font-style-tt">VasyaToolKit</span>). One of the interesting aspects of this library is that widgets are packed in each other. </p><p>A widget is some element of graphical interface. Each widget has width and height, and occupies some rectangle on the screen. Any widget in Vasya's library is of type <span class="tex-font-style-tt">Widget</span>. For simplicity we will identify the widget and its type. </p><p>Types <span class="tex-font-style-tt">HBox</span> and <span class="tex-font-style-tt">VBox</span> are derivatives of type <span class="tex-font-style-tt">Widget</span>, so they also are types <span class="tex-font-style-tt">Widget</span>. Widgets <span class="tex-font-style-tt">HBox</span> and <span class="tex-font-style-tt">VBox</span> are special. They can store other widgets. Both those widgets can use the <span class="tex-font-style-tt">pack()</span> method to pack directly in itself some other widget. Widgets of types <span class="tex-font-style-tt">HBox</span> and <span class="tex-font-style-tt">VBox</span> can store several other widgets, even several equal widgets — they will simply appear several times. As a result of using the method <span class="tex-font-style-tt">pack()</span> only the link to the packed widget is saved, that is when the packed widget is changed, its image in the widget, into which it is packed, will also change. </p><p>We shall assume that the widget <span class="tex-span"><i>a</i></span> is packed in the widget <span class="tex-span"><i>b</i></span> if there exists a chain of widgets <span class="tex-span"><i>a</i> = <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub> = <i>b</i></span>, <span class="tex-span"><i>k</i> ≥ 2</span>, for which <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is packed directly to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> for any <span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span>. In Vasya's library the situation when the widget <span class="tex-span"><i>a</i></span> is packed in the widget <span class="tex-span"><i>a</i></span> (that is, in itself) is not allowed. If you try to pack the widgets into each other in this manner immediately results in an error.</p><p>Also, the widgets <span class="tex-font-style-tt">HBox</span> and <span class="tex-font-style-tt">VBox</span> have parameters <span class="tex-font-style-tt">border</span> and <span class="tex-font-style-tt">spacing</span>, which are determined by the methods <span class="tex-font-style-tt">set_border()</span> and <span class="tex-font-style-tt">set_spacing()</span> respectively. By default both of these options equal <span class="tex-span">0</span>. </p><center> <img class="tex-graphics" src="file://5ZEuUZPy.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <p>The picture above shows how the widgets are packed into <span class="tex-font-style-tt">HBox</span> and <span class="tex-font-style-tt">VBox</span>. At that <span class="tex-font-style-tt">HBox</span> and <span class="tex-font-style-tt">VBox</span> automatically change their size depending on the size of packed widgets. As for <span class="tex-font-style-tt">HBox</span> and <span class="tex-font-style-tt">VBox</span>, they only differ in that in <span class="tex-font-style-tt">HBox</span> the widgets are packed horizontally and in <span class="tex-font-style-tt">VBox</span> — vertically. The parameter <span class="tex-font-style-tt">spacing</span> sets the distance between adjacent widgets, and <span class="tex-font-style-tt">border</span> — a frame around all packed widgets of the desired width. Packed widgets are placed exactly in the order in which the <span class="tex-font-style-tt">pack()</span> method was called for them. If within <span class="tex-font-style-tt">HBox</span> or <span class="tex-font-style-tt">VBox</span> there are no packed widgets, their sizes are equal to <span class="tex-span">0 × 0</span>, regardless of the options <span class="tex-font-style-tt">border</span> and <span class="tex-font-style-tt">spacing</span>. </p><p>The construction of all the widgets is performed using a scripting language <span class="tex-font-style-tt">VasyaScript</span>. The description of the language can be found in the input data. </p><p>For the final verification of the code Vasya asks you to write a program that calculates the sizes of all the widgets on the source code in the language of <span class="tex-font-style-tt">VasyaScript</span>. </p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> — the number of instructions (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Next <span class="tex-span"><i>n</i></span> lines contain instructions in the language <span class="tex-font-style-tt">VasyaScript</span> — one instruction per line. There is a list of possible instructions below. </p><ul><li> "<span class="tex-font-style-tt">Widget [name]([x],[y])</span>" — create a new widget <span class="tex-font-style-tt">[name]</span> of the type <span class="tex-font-style-tt">Widget</span> possessing the width of <span class="tex-font-style-tt">[x]</span> units and the height of <span class="tex-font-style-tt">[y]</span> units. </li><li> "<span class="tex-font-style-tt">HBox [name]</span>" — create a new widget <span class="tex-font-style-tt">[name]</span> of the type <span class="tex-font-style-tt">HBox</span>. </li><li> "<span class="tex-font-style-tt">VBox [name]</span>" — create a new widget <span class="tex-font-style-tt">[name]</span> of the type <span class="tex-font-style-tt">VBox</span>. </li><li> "<span class="tex-font-style-tt">[name1].pack([name2])</span>" — pack the widget <span class="tex-font-style-tt">[name2]</span> in the widget <span class="tex-font-style-tt">[name1]</span>. At that, the widget <span class="tex-font-style-tt">[name1]</span> must be of type <span class="tex-font-style-tt">HBox</span> or <span class="tex-font-style-tt">VBox</span>. </li><li> "<span class="tex-font-style-tt">[name].set_border([x])</span>" — set for a widget <span class="tex-font-style-tt">[name]</span> the <span class="tex-font-style-tt">border</span> parameter to <span class="tex-font-style-tt">[x]</span> units. The widget <span class="tex-font-style-tt">[name]</span> must be of type <span class="tex-font-style-tt">HBox</span> or <span class="tex-font-style-tt">VBox</span>. </li><li> "<span class="tex-font-style-tt">[name].set_spacing([x])</span>" — set for a widget <span class="tex-font-style-tt">[name]</span> the <span class="tex-font-style-tt">spacing</span> parameter to <span class="tex-font-style-tt">[x]</span> units. The widget <span class="tex-font-style-tt">[name]</span> must be of type <span class="tex-font-style-tt">HBox</span> or <span class="tex-font-style-tt">VBox</span>. </li></ul> <p>All instructions are written without spaces at the beginning and at the end of the string. The words inside the instruction are separated by exactly one space. There are no spaces directly before the numbers and directly after them. </p><p>The case matters, for example, "<span class="tex-font-style-tt">wiDget x</span>" is not a correct instruction. The case of the letters is correct in the input data.</p><p>All names of the widgets consist of lowercase Latin letters and has the length from <span class="tex-span">1</span> to <span class="tex-span">10</span> characters inclusive. The names of all widgets are pairwise different. All numbers in the script are integers from <span class="tex-span">0</span> to <span class="tex-span">100</span> inclusive</p><p>It is guaranteed that the above-given script is correct, that is that all the operations with the widgets take place after the widgets are created and no widget is packed in itself. It is guaranteed that the script creates at least one widget. </p></div><div class="output-specification"><p>For each widget print on a single line its name, width and height, separated by spaces. The lines must be ordered lexicographically by a widget's name. </p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use <span class="tex-font-style-tt">cout</span> stream (also you may use <span class="tex-font-style-tt">%I64d</span> specificator)</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> — the number of instructions (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Next <span class="tex-span"><i>n</i></span> lines contain instructions in the language <span class="tex-font-style-tt">VasyaScript</span> — one instruction per line. There is a list of possible instructions below. </p><ul><li> "<span class="tex-font-style-tt">Widget [name]([x],[y])</span>" — create a new widget <span class="tex-font-style-tt">[name]</span> of the type <span class="tex-font-style-tt">Widget</span> possessing the width of <span class="tex-font-style-tt">[x]</span> units and the height of <span class="tex-font-style-tt">[y]</span> units. </li><li> "<span class="tex-font-style-tt">HBox [name]</span>" — create a new widget <span class="tex-font-style-tt">[name]</span> of the type <span class="tex-font-style-tt">HBox</span>. </li><li> "<span class="tex-font-style-tt">VBox [name]</span>" — create a new widget <span class="tex-font-style-tt">[name]</span> of the type <span class="tex-font-style-tt">VBox</span>. </li><li> "<span class="tex-font-style-tt">[name1].pack([name2])</span>" — pack the widget <span class="tex-font-style-tt">[name2]</span> in the widget <span class="tex-font-style-tt">[name1]</span>. At that, the widget <span class="tex-font-style-tt">[name1]</span> must be of type <span class="tex-font-style-tt">HBox</span> or <span class="tex-font-style-tt">VBox</span>. </li><li> "<span class="tex-font-style-tt">[name].set_border([x])</span>" — set for a widget <span class="tex-font-style-tt">[name]</span> the <span class="tex-font-style-tt">border</span> parameter to <span class="tex-font-style-tt">[x]</span> units. The widget <span class="tex-font-style-tt">[name]</span> must be of type <span class="tex-font-style-tt">HBox</span> or <span class="tex-font-style-tt">VBox</span>. </li><li> "<span class="tex-font-style-tt">[name].set_spacing([x])</span>" — set for a widget <span class="tex-font-style-tt">[name]</span> the <span class="tex-font-style-tt">spacing</span> parameter to <span class="tex-font-style-tt">[x]</span> units. The widget <span class="tex-font-style-tt">[name]</span> must be of type <span class="tex-font-style-tt">HBox</span> or <span class="tex-font-style-tt">VBox</span>. </li></ul> <p>All instructions are written without spaces at the beginning and at the end of the string. The words inside the instruction are separated by exactly one space. There are no spaces directly before the numbers and directly after them. </p><p>The case matters, for example, "<span class="tex-font-style-tt">wiDget x</span>" is not a correct instruction. The case of the letters is correct in the input data.</p><p>All names of the widgets consist of lowercase Latin letters and has the length from <span class="tex-span">1</span> to <span class="tex-span">10</span> characters inclusive. The names of all widgets are pairwise different. All numbers in the script are integers from <span class="tex-span">0</span> to <span class="tex-span">100</span> inclusive</p><p>It is guaranteed that the above-given script is correct, that is that all the operations with the widgets take place after the widgets are created and no widget is packed in itself. It is guaranteed that the script creates at least one widget. </p>

## Output

<p>For each widget print on a single line its name, width and height, separated by spaces. The lines must be ordered lexicographically by a widget's name. </p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use <span class="tex-font-style-tt">cout</span> stream (also you may use <span class="tex-font-style-tt">%I64d</span> specificator)</p>





```input1
12
Widget me(50,40)
VBox grandpa
HBox father
grandpa.pack(father)
father.pack(me)
grandpa.set_border(10)
grandpa.set_spacing(20)
Widget brother(30,60)
father.pack(brother)
Widget friend(20,60)
Widget uncle(100,20)
grandpa.pack(uncle)

```




```input2
15
Widget pack(10,10)
HBox dummy
HBox x
VBox y
y.pack(dummy)
y.set_border(5)
y.set_spacing(55)
dummy.set_border(10)
dummy.set_spacing(20)
x.set_border(10)
x.set_spacing(10)
x.pack(pack)
x.pack(dummy)
x.pack(pack)
x.set_border(0)

```




```output1
brother 30 60
father 80 60
friend 20 60
grandpa 120 120
me 50 40
uncle 100 20

```




```output2
dummy 0 0
pack 10 10
x 40 10
y 10 10

```



## Note

<p>In the first sample the widgets are arranged as follows: </p><center> <img class="tex-graphics" src="file://XBesbNH7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
