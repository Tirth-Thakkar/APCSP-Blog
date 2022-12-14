---
keywords: fastai
description: Developing and Writing Procedures Lesson
title: Unit 3 Sections 12-13
toc: true
badges: false
tags: [chapter3, week15]
categories: [chapter3, week15]
nb_path: _notebooks/2022-12-07-developing-procedures.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-12-07-developing-procedures.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Calling-Procedures">Calling Procedures<a class="anchor-link" href="#Calling-Procedures"> </a></h2><p>Slide 1:</p>
<ul>
<li>A <mark>procedure</mark> is a named group of programming instructions that may have parameters and return values.</li>
<li>Procedures are referred to by different names, such as <mark>method</mark> or <mark>function</mark>, depending on the programing language.</li>
<li>Parameters are input values of a procedure. <mark>Arugments</mark> specify the values of the parameters when procedure is called.</li>
<li>A procedure call interrupts the <mark>sequential</mark> execution of statements causing the program to execute the statements within the procedure before continuing. One the last statement in the procedure (or a return statement) has executed, flow or control is returned to the point immediately following where the procedure was <mark>called</mark>.</li>
</ul>
<p>Slide 2:</p>
<ul>
<li>When calling procedures, it's important to take notice to whether it returns data, or a block of <mark>statements</mark>.</li>
<li>If the procedure just returns a block of statements, you call the procedure by referring to the procedure name, and inputting the <mark>arguments</mark>.</li>
<li>If the procedure returns some sort of data like a <mark>boolean</mark> or <mark>value</mark>, then you will assign that value to a variable</li>
</ul>
<p>Slide 3:</p>
<ul>
<li>Assume the Temperature outside is Fahrenheit. </li>
<li>The procedure <mark>convertFahrenheit</mark> is intended to convert from Fahrenheit to Celsius.</li>
<li>Convert the following psuedocode to python</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">convertFahrenheit</span><span class="p">(</span><span class="n">temperature</span><span class="p">):</span>
    <span class="n">celsius</span> <span class="o">=</span> <span class="n">temperature</span> <span class="o">-</span> <span class="mi">32</span>
    <span class="n">celsius</span> <span class="o">=</span> <span class="n">celsius</span> <span class="o">*</span> <span class="mi">5</span><span class="o">/</span><span class="mi">9</span>
    <span class="k">return</span> <span class="n">celsius</span>

<span class="n">outsideTemp</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter temperature in celsius&quot;</span><span class="p">)</span>
<span class="n">outsideTemp</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">outsideTemp</span><span class="p">)</span>
<span class="n">convertFahrenheit</span><span class="p">(</span><span class="n">outsideTemp</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">



<div class="output_text output_subarea output_execute_result">
<pre>0.5555555555555556</pre>
</div>

</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Developing-Procedures">Developing Procedures<a class="anchor-link" href="#Developing-Procedures"> </a></h2><p>Slide 8:</p>
<p>Picking a <mark>decriptive</mark> name is important in case you revisit the code later on (separate words with capitals)
There are 2 different types of procedures- ones that return a value and those that simply execute a block of statements
Steps of developing procedure: picking a useful name, thinking of parameters (what data does the procedure need to know), making a flowchart or writing procedure in pseudocode, and actually developing the procedure.</p>
<p>Slide 9:</p>
<p>In this example, a teacher is writing a program that will replace the grade on a previous quiz if the new grade is better than the previous.</p>
<ul>
<li>What would be a good name for this procedure?</li>
<li>What parameters do we need for this procedure?</li>
<li>Try writing this procedure out in python based on the given pseudocode</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="procedure-goes-here">procedure goes here<a class="anchor-link" href="#procedure-goes-here"> </a></h1><p>currentGrade &lt;- currentPoints / 40
currentGrade &lt;- current Grade * 100
if currentGrade &gt; quizGrade
    quizGrade &lt;- currentGrade</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">quiz_grader</span><span class="p">():</span>
    <span class="n">currentPoints</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Amount of points scored:&quot;</span><span class="p">))</span>
    <span class="n">totalPoints</span> <span class="o">=</span> <span class="nb">int</span><span class="p">((</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Amount of  points possble&quot;</span><span class="p">)))</span>
    <span class="n">grade</span> <span class="o">=</span> <span class="n">currentPoints</span><span class="o">/</span><span class="n">totalPoints</span> <span class="o">*</span> <span class="mi">100</span>
    <span class="nb">print</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">grade</span><span class="p">)</span><span class="o">+</span><span class="s2">&quot;% was the score this student recieved on this quiz they scored &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">currentPoints</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; out of &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">totalPoints</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; points.&quot;</span><span class="p">)</span> 
<span class="n">quiz_grader</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>5.0% was the score this student recieved on this quiz they scored 2 out of 40 points.
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Procedural-Abstraction">Procedural Abstraction<a class="anchor-link" href="#Procedural-Abstraction"> </a></h2><ul>
<li>One type of abstraction is <mark>procedural</mark> abstraction which provides a name for a process and allows a procedure to be used only knowing what it does and not how it does it</li>
<li>This is very helpful in managing <mark>complexity</mark> in a program</li>
<li>Subdivision of a program into separate subprograms is called <mark>modularity</mark></li>
<li>A procedural abstraction may <mark>extract</mark> shared features to generalize functionality instead of duplicating code. This allows for program reuse, which helps manage complexity</li>
<li>When a pre-written procedure is called, you don???t necessarily need to know the details of this, just what it does and how to call it</li>
<li>Simply, procedural abstraction is naming and calling a prewritten procedure</li>
<li>Making sure to include the right arguments so the procedure can do what its supposed to do is crucial</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Complexity-Example">Complexity Example<a class="anchor-link" href="#Complexity-Example"> </a></h2><p>One of the biggest advantages of procedural abstraction is managing complexity.</p>
<p>Think about the process of simplifying the code?
What do you think the advantage of the code segment on the left is?</p>
<table>
<thead><tr>
<th>Code Segment 1</th>
<th>Code Segment 2</th>
</tr>
</thead>
<tbody>
<tr>
<td>ROTATE_LEFT()</td>
<td>detourLeft()</td>
</tr>
</tbody>
</table>
<p>MOVE_FORWARD()|turnCorner()| 
ROTATE_RIGHT  |MOVE_FORWARD()| 
MOVE_FORWARD()|MOVE_FORWARD()|
MOVE_FORWARD()
ROTATE_RIGHT()
MOVE_FORWARD()
ROTATE_LEFT()
MOVE_FORWARD()
ROTATE_LEFT()
MOVE_FORWARD()
MOVE_FORWARD
MOVE_FORWARD()</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Hacks">Hacks<a class="anchor-link" href="#Hacks"> </a></h2><ul>
<li>Write a python procedure about something which can help you in school, for example the teacher???s function we spoke about earlier.</li>
<li>Points will be awarded based on creativity and functionality</li>
<li>0.1 points will be deducted for late submissions</li>
<li>Submit the notes with all blanks filled in (scored out of 0.5 points) and the python procedure (scored out of 0.5 points) by Monday 12/12 at 11:59 PM.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">time</span>

<span class="k">def</span> <span class="nf">AssignmentTimer</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;You have &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">x</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; minute/s to work on this assignment.&quot;</span><span class="p">)</span>
    <span class="k">try</span><span class="p">:</span>
        <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="n">x</span><span class="o">*</span><span class="mi">60</span><span class="p">)</span>
    <span class="k">except</span> <span class="ne">KeyboardInterrupt</span><span class="p">:</span>
        <span class="c1"># allows the user to cancel the timer</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Timer cancelled.&quot;</span><span class="p">)</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Time is up! Take a break!&quot;</span><span class="p">)</span>

<span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
    <span class="n">minutes</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of minutes you would like to work on your assignment: &quot;</span><span class="p">))</span>
    <span class="n">AssignmentTimer</span><span class="p">(</span><span class="n">minutes</span><span class="p">)</span>

    <span class="c1"># Allows typos in the user&#39;s response if they want another timer</span>
    <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
        <span class="n">response</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Do you want to start another timer? (yes/no)&quot;</span><span class="p">)</span>
        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;no&quot;</span><span class="p">:</span>
            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Goodbye!&quot;</span><span class="p">)</span>
            <span class="k">break</span>
        <span class="k">elif</span> <span class="n">response</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;yes&quot;</span><span class="p">:</span>
            <span class="k">break</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid response. Please enter &#39;yes&#39; or &#39;no&#39;.&quot;</span><span class="p">)</span>

    <span class="c1"># Stops the loop if the user doesn&#39;t want another timer</span>
    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;no&quot;</span><span class="p">:</span>
        <span class="k">break</span>

    <span class="c1"># Demonstration of an algorithm that has a use case that could be useful for school in a way</span>
    <span class="c1"># that allows the user to input the number of minutes they want to work on their assignment</span>
    <span class="c1"># and then the program will start a timer for that amount of time and then the user can</span>
    <span class="c1"># cancel the timer if they want to stop working on their assignment or the timer will</span>
    <span class="c1"># automatically end after the amount of time the user inputted and if they don&#39;t want another timer.</span>
    <span class="c1"># Allows the user to manage thier time better and be more productive throug taking regular breaks</span>
    <span class="c1"># and manage the amount of time certain assignments take to complete.</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>You have 1 minute/s to work on this assignment.
Time is up! Take a break!
Invalid response. Please enter &#39;yes&#39; or &#39;no&#39;.
You have 2 minute/s to work on this assignment.
Time is up! Take a break!
You have 69420 minute/s to work on this assignment.
Timer cancelled.
Goodbye!
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

