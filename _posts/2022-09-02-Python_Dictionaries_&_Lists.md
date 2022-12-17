---
keywords: fastai
description: Information on peer team 
title: Information
toc: true
branch: master
comments: true
image: /images/Information.jpg
categories: [python]
nb_path: _notebooks/2022-09-02-Python_Dictionaries_&_Lists.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-09-02-Python_Dictionaries_&_Lists.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">Peers_Info</span> <span class="o">=</span> <span class="p">[]</span>

<span class="n">Peers_Info</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;First_Name&quot;</span><span class="p">:</span> <span class="s2">&quot;Tirth&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Middle_Name/Initial&quot;</span><span class="p">:</span><span class="s2">&quot;S.&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Last_Name&quot;</span><span class="p">:</span> <span class="s2">&quot;Thakkar&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Residence&quot;</span><span class="p">:</span> <span class="s2">&quot;San Diego&quot;</span><span class="p">,</span>
    <span class="s2">&quot;DOB&quot;</span><span class="p">:</span> <span class="s2">&quot;December 26, 2005&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Grade&quot;</span><span class="p">:</span> <span class="s2">&quot;11th&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Email&quot;</span><span class="p">:</span> <span class="s2">&quot;tirth1226@gmail.com&quot;</span><span class="p">,</span>
<span class="p">})</span>

<span class="n">Peers_Info</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;First_Name&quot;</span><span class="p">:</span> <span class="s2">&quot;Mirza&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Middle_Name/Initial&quot;</span><span class="p">:</span> <span class="s2">&quot;Haseeb&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Last_Name&quot;</span><span class="p">:</span> <span class="s2">&quot;Beg&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Residence&quot;</span><span class="p">:</span> <span class="s2">&quot;San Diego&quot;</span><span class="p">,</span>
    <span class="s2">&quot;DOB&quot;</span><span class="p">:</span> <span class="s2">&quot;December 6th, 2007&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Grade&quot;</span><span class="p">:</span> <span class="s2">&quot;10th&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Email&quot;</span><span class="p">:</span> <span class="s2">&quot;mirzahbeg123@gmail.com&quot;</span><span class="p">,</span>
<span class="p">})</span>

<span class="nb">print</span><span class="p">(</span><span class="n">Peers_Info</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[{&#39;First_Name&#39;: &#39;Tirth&#39;, &#39;Middle_Name/Initial&#39;: &#39;S.&#39;, &#39;Last_Name&#39;: &#39;Thakkar&#39;, &#39;Residence&#39;: &#39;San Diego&#39;, &#39;DOB&#39;: &#39;December 26, 2005&#39;, &#39;Grade&#39;: &#39;11th&#39;, &#39;Email&#39;: &#39;tirth1226@gmail.com&#39;}, {&#39;First_Name&#39;: &#39;Mirza&#39;, &#39;Middle_Name/Initial&#39;: &#39;Haseeb&#39;, &#39;Last_Name&#39;: &#39;Beg&#39;, &#39;Residence&#39;: &#39;San Diego&#39;, &#39;DOB&#39;: &#39;December 6th, 2007&#39;, &#39;Grade&#39;: &#39;10th&#39;, &#39;Email&#39;: &#39;mirzahbeg123@gmail.com&#39;}]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Formatting">Formatting<a class="anchor-link" href="#Formatting"> </a></h3><p>Way to organize and format the data.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">formatting</span><span class="p">(</span><span class="n">d_rec</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\033</span><span class="s2">[1m&quot;</span><span class="p">,</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;First_Name&quot;</span><span class="p">],</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;Middle_Name/Initial&quot;</span><span class="p">],</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;Last_Name&quot;</span><span class="p">],</span> <span class="s2">&quot;</span><span class="se">\x1b</span><span class="s2">[0m&quot;</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\033</span><span class="s2">[4m&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\t</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;Residence:&quot;</span><span class="p">,</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;Residence&quot;</span><span class="p">],</span> <span class="s2">&quot;</span><span class="se">\x1b</span><span class="s2">[0m&quot;</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\033</span><span class="s2">[4m&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\t</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;Birth Day:&quot;</span><span class="p">,</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;DOB&quot;</span><span class="p">],</span> <span class="s2">&quot;</span><span class="se">\x1b</span><span class="s2">[0m&quot;</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\033</span><span class="s2">[4m&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\t</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;Grade:&quot;</span><span class="p">,</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;Grade&quot;</span><span class="p">],</span> <span class="s2">&quot;</span><span class="se">\x1b</span><span class="s2">[0m&quot;</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\033</span><span class="s2">[4m&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\t</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;Email:&quot;</span><span class="p">,</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;Email&quot;</span><span class="p">],</span> <span class="s2">&quot;</span><span class="se">\x1b</span><span class="s2">[0m&quot;</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">()</span>

<span class="k">def</span> <span class="nf">printing</span><span class="p">():</span>
    <span class="k">for</span> <span class="n">index</span> <span class="ow">in</span> <span class="n">Peers_Info</span><span class="p">:</span>
        <span class="n">formatting</span><span class="p">(</span><span class="n">index</span><span class="p">)</span>

<span class="n">printing</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre><span class="ansi-bold"> Tirth S. Thakkar </span>
<span class="ansi-underline"> 	 Residence: San Diego </span>
<span class="ansi-underline"> 	 Birth Day: December 26, 2005 </span>
<span class="ansi-underline"> 	 Grade: 11th </span>
<span class="ansi-underline"> 	 Email: tirth1226@gmail.com </span>

<span class="ansi-bold"> Mirza Haseeb Beg </span>
<span class="ansi-underline"> 	 Residence: San Diego </span>
<span class="ansi-underline"> 	 Birth Day: December 6th, 2007 </span>
<span class="ansi-underline"> 	 Grade: 10th </span>
<span class="ansi-underline"> 	 Email: mirzahbeg123@gmail.com </span>

</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Reversal">Reversal<a class="anchor-link" href="#Reversal"> </a></h3><p>Way to reverse the data.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">Peers_Info</span><span class="o">.</span><span class="n">reverse</span><span class="p">()</span>

<span class="n">printing</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre><span class="ansi-bold"> Mirza Haseeb Beg </span>
<span class="ansi-underline"> 	 Residence: San Diego </span>
<span class="ansi-underline"> 	 Birth Day: December 6th, 2007 </span>
<span class="ansi-underline"> 	 Grade: 10th </span>
<span class="ansi-underline"> 	 Email: mirzahbeg123@gmail.com </span>

<span class="ansi-bold"> Tirth S. Thakkar </span>
<span class="ansi-underline"> 	 Residence: San Diego </span>
<span class="ansi-underline"> 	 Birth Day: December 26, 2005 </span>
<span class="ansi-underline"> 	 Grade: 11th </span>
<span class="ansi-underline"> 	 Email: tirth1226@gmail.com </span>

</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 
