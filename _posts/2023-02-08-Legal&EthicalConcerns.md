---
keywords: fastai
description: A reflection on encryption and personal information
title: Safe Computing - 5.6
toc: true
badges: false
tags: [week22]
categories: [week22]
nb_path: _notebooks/2023-02-08-Legal&EthicalConcerns.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2023-02-08-Legal&EthicalConcerns.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Personal-Identifiable-Information-(PII)">Personal Identifiable Information (PII)<a class="anchor-link" href="#Personal-Identifiable-Information-(PII)"> </a></h2><ul>
<li>PII is any information that can be used to identify, contact, or locate a single person, or to identify an individual in context.</li>
<li>PII can be made up of a variety of different kinds of data, including names, addresses, phone numbers, email addresses, social security numbers, and other identifiers. </li>
<li>PII can also include information about a person’s physical or mental health, financial information, or other information that can be used to identify a person.</li>
<li>The kind of PII that we've seen in our personal projects is the storing of use data in a login system such as the user's information, uid, username, password, etc. This kind of information can tie an account to a person's identity.</li>
<li>We have also seen personal information when signing up for services that we use such as accounts for microsoft, google, github, etc. which store emails, phone numbers, often address and other information while setting up the tools that we use to create our projects. </li>
</ul>
<h2 id="Feeling-PII-&amp;-Personal-Exposure">Feeling PII &amp; Personal Exposure<a class="anchor-link" href="#Feeling-PII-&amp;-Personal-Exposure"> </a></h2><ul>
<li>My feelings about PII is that they are needed for the creation for accounts and are the only way to create a way in a single person can be tied to a single account. My personal exposure to these concepts is through the creation of accounts for services that I use such as github, google, microsoft, youtube, etc. This will mean that if there is a data breach, my information will be exposed to the public and can be used to steal content such as my identity, my credit card information, my bank account information, etc.</li>
</ul>
<h2 id="Good-Vs.-Bad-Password">Good Vs. Bad Password<a class="anchor-link" href="#Good-Vs.-Bad-Password"> </a></h2><ul>
<li>A good password is one that are random, complex, and long as it makes them harder to decrypt and social engineer and makes them harder to guess or trick out of you. Bad passwords are ones that are easy to guess, easy to social engineer, or easy to trick out of you such as your name, your birthday, your address, your phone number, pet's name, etc. </li>
</ul>
<h2 id="Symmetric-&amp;-Asymmetric-Encryption">Symmetric &amp; Asymmetric Encryption<a class="anchor-link" href="#Symmetric-&amp;-Asymmetric-Encryption"> </a></h2><ul>
<li><p>Symmetric encryption is a type of encryption where the same key is used to encrypt and decrypt the data. This is the most common type of encryption that we see in our daily lives such as the encryption of our passwords. This means that there is a faster encryption and decryption process as the same key is used for both. Example Symmetric Encryption: AES, DES, 3DES, etc.</p>
</li>
<li><p>Asymmetric encryption is a type of encryption where there are two keys, a public key and a private key. The public key is used to encrypt the data and the private key is used to decrypt the data. This is the type of encryption that we see in our daily lives when we use https websites such as google, github, etc.
Example Asymmetric Encryption: RSA, ECC, etc.</p>
</li>
</ul>
<h2 id="AWS-Deployment">AWS Deployment<a class="anchor-link" href="#AWS-Deployment"> </a></h2><ul>
<li>We used private and public ssh keys while deploying our project to AWS we also created a .pem file that we used to ssh into our instance. We used some basic encryption in our AWS project. However, other than that I don't think we used any other encryption in our project as we were not knowledgeable enough to do so.</li>
</ul>
<h2 id="How-I-got-Phished">How I got Phished<a class="anchor-link" href="#How-I-got-Phished"> </a></h2><ul>
<li>I was once sent an email by a group claiming to be Wells Fargo Customer Service. The email was sent to my personal email and was asking me to verify my account information. I was asked to click on a link and enter my information. However, considering the fact that I don't have a Wells Fargo account, I knew that this was a phishing email. However, had I been tricked I may have entered in sensitive information such as my social security number, my bank account information, etc.</li>
</ul>

</div>
</div>
</div>
</div>
 
