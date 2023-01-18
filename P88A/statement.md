## Description

<div><p>Vasya studies music. </p><p>He has learned lots of interesting stuff. For example, he knows that there are 12 notes: <span class="tex-font-style-tt">C</span>, <span class="tex-font-style-tt">C#</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">D#</span>, <span class="tex-font-style-tt">E</span>, <span class="tex-font-style-tt">F</span>, <span class="tex-font-style-tt">F#</span>, <span class="tex-font-style-tt">G</span>, <span class="tex-font-style-tt">G#</span>, <span class="tex-font-style-tt">A</span>, <span class="tex-font-style-tt">B</span>, <span class="tex-font-style-tt">H</span>. He also knows that the notes are repeated cyclically: after <span class="tex-font-style-tt">H</span> goes <span class="tex-font-style-tt">C</span> again, and before <span class="tex-font-style-tt">C</span> stands <span class="tex-font-style-tt">H</span>. We will consider the <span class="tex-font-style-tt">C</span> note in the row's beginning and the <span class="tex-font-style-tt">C</span> note after the <span class="tex-font-style-tt">H</span> similar and we will identify them with each other. The distance between the notes along the musical scale is measured in tones: between two consecutive notes there's exactly one semitone, that is, 0.5 tone. The distance is taken from the lowest tone to the uppest one, that is, the distance between <span class="tex-font-style-tt">C</span> and <span class="tex-font-style-tt">E</span> is 4 semitones and between <span class="tex-font-style-tt">E</span> and <span class="tex-font-style-tt">C</span> is 8 semitones</p><p>Vasya also knows what a chord is. A chord is an unordered set of no less than three notes. However, for now Vasya only works with triads, that is with the chords that consist of exactly three notes. He can already distinguish between two types of triads — major and minor.</p><p>Let's define a major triad. Let the triad consist of notes <span class="tex-span"><i>X</i></span>, <span class="tex-span"><i>Y</i></span> and <span class="tex-span"><i>Z</i></span>. If we can order the notes so as the distance along the musical scale between <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> equals 4 semitones and the distance between <span class="tex-span"><i>Y</i></span> and <span class="tex-span"><i>Z</i></span> is 3 semitones, then the triad is major. The distance between <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Z</i></span>, accordingly, equals 7 semitones.</p><p>A minor triad is different in that the distance between <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> should be 3 semitones and between <span class="tex-span"><i>Y</i></span> and <span class="tex-span"><i>Z</i></span> — 4 semitones.</p><p>For example, the triad "<span class="tex-font-style-tt">C E G</span>" is major: between <span class="tex-font-style-tt">C</span> and <span class="tex-font-style-tt">E</span> are 4 semitones, and between <span class="tex-font-style-tt">E</span> and <span class="tex-font-style-tt">G</span> are 3 semitones. And the triplet "<span class="tex-font-style-tt">C# B F</span>" is minor, because if we order the notes as "<span class="tex-font-style-tt">B C# F</span>", than between <span class="tex-font-style-tt">B</span> and <span class="tex-font-style-tt">C#</span> will be 3 semitones, and between <span class="tex-font-style-tt">C#</span> and <span class="tex-font-style-tt">F</span> — 4 semitones.</p><p>Help Vasya classify the triad the teacher has given to him.</p></div><div class="input-specification"><p>The only line contains 3 space-separated notes in the above-given notation.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">major</span>" if the chord is major, "<span class="tex-font-style-tt">minor</span>" if it is minor, and "<span class="tex-font-style-tt">strange</span>" if the teacher gave Vasya some weird chord which is neither major nor minor. Vasya promises you that the answer will always be unambiguous. That is, there are no chords that are both major and minor simultaneously.</p></div>

## Input

<p>The only line contains 3 space-separated notes in the above-given notation.</p>

## Output

<p>Print "<span class="tex-font-style-tt">major</span>" if the chord is major, "<span class="tex-font-style-tt">minor</span>" if it is minor, and "<span class="tex-font-style-tt">strange</span>" if the teacher gave Vasya some weird chord which is neither major nor minor. Vasya promises you that the answer will always be unambiguous. That is, there are no chords that are both major and minor simultaneously.</p>





```input1
C E G

```




```input2
C# B F

```




```input3
A B H

```




```output1
major

```




```output2
minor

```




```output3
strange

```


