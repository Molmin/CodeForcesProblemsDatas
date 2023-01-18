## Description

<div><p>After the contest in comparing numbers, Shapur's teacher found out that he is a real genius and that no one could possibly do the calculations faster than him even using a super computer!</p><p>Some days before the contest, the teacher took a very simple-looking exam and all his <span class="tex-span"><i>n</i></span> students took part in the exam. The teacher gave them <span class="tex-span">3</span> strings and asked them to <span class="tex-font-style-underline">concatenate</span> them. Concatenating strings means to put them in some arbitrary order one after the other. For example from concatenating <span class="tex-font-style-tt">Alireza</span> and <span class="tex-font-style-tt">Amir</span> we can get to <span class="tex-font-style-tt">AlirezaAmir</span> or <span class="tex-font-style-tt">AmirAlireza</span> depending on the order of concatenation.</p><p>Unfortunately enough, the teacher forgot to ask students to concatenate their strings in a pre-defined order so each student did it the way he/she liked.</p><p>Now the teacher knows that Shapur is such a fast-calculating genius boy and asks him to correct the students' papers.</p><p>Shapur is not good at doing such a time-taking task. He rather likes to finish up with it as soon as possible and take his time to solve 3-SAT in polynomial time. Moreover, the teacher has given some advice that Shapur has to follow. Here's what the teacher said: </p><ul> <li> As I expect you know, the strings I gave to my students (including you) contained only lowercase and uppercase Persian Mikhi-Script letters. These letters are too much like Latin letters, so to make your task much harder I converted all the initial strings and all of the students' answers to Latin. </li><li> As latin alphabet has much less characters than Mikhi-Script, I added three odd-looking characters to the answers, these include "<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">;</span>" and "<span class="tex-font-style-tt">_</span>". These characters are my own invention of course! And I call them <span class="tex-font-style-underline">Signs</span>. </li><li> The length of all initial strings was less than or equal to <span class="tex-span">100</span> and the lengths of my students' answers are less than or equal to <span class="tex-span">600</span> </li><li> My son, not all students are genius as you are. It is quite possible that they make minor mistakes changing case of some characters. For example they may write <span class="tex-font-style-tt">ALiReZaAmIR</span> instead of <span class="tex-font-style-tt">AlirezaAmir</span>. Don't be picky and ignore these mistakes. </li><li> Those signs which I previously talked to you about are not important. You can ignore them, since many students are in the mood for adding extra signs or forgetting about a sign. So something like <span class="tex-font-style-tt">Iran;;--</span> is the same as <span class="tex-font-style-tt">--;IRAN</span> </li><li> You should indicate for any of my students if his answer was right or wrong. Do this by writing "<span class="tex-font-style-tt">WA</span>" for Wrong answer or "<span class="tex-font-style-tt">ACC</span>" for a correct answer. </li><li> I should remind you that none of the strings (initial strings or answers) are empty. </li><li> Finally, do these as soon as possible. You have less than <span class="tex-span">2</span> hours to complete this. </li></ul> </div><div class="input-specification"><p>The first three lines contain a string each. These are the initial strings. They consists only of lowercase and uppercase Latin letters and signs ("<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">;</span>" and "<span class="tex-font-style-tt">_</span>"). All the initial strings have length from 1 to 100, inclusively.</p><p>In the fourth line there is a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 1000</span>), the number of students.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain a student's answer each. It is guaranteed that the answer meets what the teacher said. Each answer iconsists only of lowercase and uppercase Latin letters and signs ("<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">;</span>" and "<span class="tex-font-style-tt">_</span>"). Length is from 1 to 600, inclusively.</p></div><div class="output-specification"><p>For each student write in a different line. Print "<span class="tex-font-style-tt">WA</span>" if his answer is wrong or "<span class="tex-font-style-tt">ACC</span>" if his answer is OK.</p></div>

## Input

<p>The first three lines contain a string each. These are the initial strings. They consists only of lowercase and uppercase Latin letters and signs ("<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">;</span>" and "<span class="tex-font-style-tt">_</span>"). All the initial strings have length from 1 to 100, inclusively.</p><p>In the fourth line there is a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 1000</span>), the number of students.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain a student's answer each. It is guaranteed that the answer meets what the teacher said. Each answer iconsists only of lowercase and uppercase Latin letters and signs ("<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">;</span>" and "<span class="tex-font-style-tt">_</span>"). Length is from 1 to 600, inclusively.</p>

## Output

<p>For each student write in a different line. Print "<span class="tex-font-style-tt">WA</span>" if his answer is wrong or "<span class="tex-font-style-tt">ACC</span>" if his answer is OK.</p>





```input1
Iran_
Persian;
W_o;n;d;e;r;f;u;l;
7
WonderfulPersianIran
wonderful_PersIAN_IRAN;;_
WONDERFUL___IRAN__PERSIAN__;;
Ira__Persiann__Wonderful
Wonder;;fulPersian___;I;r;a;n;
__________IranPersianWonderful__________
PersianIran_is_Wonderful

```




```input2
Shapur;;
is___
a_genius
3
Shapur__a_is___geniUs
is___shapur___a__Genius;
Shapur;;is;;a;;geni;;us;;

```




```output1
ACC
ACC
ACC
WA
ACC
ACC
WA

```




```output2
WA
ACC
ACC

```


