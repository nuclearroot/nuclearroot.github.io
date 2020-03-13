---
layout: default
---

# My OSCP experience

I wanted to take OSCP to challenge myself and learn something new that has always interested me. When I began I didn't really know where to start, so hopefully this blog post will give people thinking of taking the exam some insight.

## My prior experience

I have worked in InfoSec for around 3 years, most recently I have been working as a SOC Analyst, in the worst case scenrio, defending against the sort of attacks one might learn in their OSCP studies. I felt like doing OSCP would better help me notice malicious behavior, which in some ways it did. 

I held the CompTIA Network+, Security+ and CySA+ certifications prior to taking the OSCP. It would be fair to say I had a general idea of some of the attacks, but no clue how to perform one. Even the concepts of reverse shells were beyond me when I began. My linux experience wasn't too great, I could cd around directories and list files, but that was probably about it. 

## What did I use to study? 

I will go into some more detail about these resources after, but I used Virtual Hacking Labs, Hack the Box, TryHackMe, PWK, Ippsec Videos and Tib3rius' privelege escalation courses.

### Virtual Hacking Labs

<a href="https://www.virtualhackinglabs.com/">Virtual Hacking Labs</a>

Virtual Hacking Labs was my intial exposure into the world of hacking. I bought the 3 month package, which comes with the 3 months in the labs and a courseware PDF. The courseware was very easy for me to follow and understand, it really holds your hand to make sure you understand what it is trying to teach. The machines in the labs have 3 ranks, Beginner, Advanced and Advanced+, so you can start easy and work your way up. There are slight nudges for the machines in the control panel, except for the Advanced+ where you are left on your own to try figure them out. I think the privilege escalation part of the course and labs could use some more variety, however I still think this is a great resource and part of the reason I passed.

### Hack The Box

<a href="https://www.hackthebox.eu/">Hack The Box</a>

I'm sure the vast majority have already heard of Hack The Box. It's a great site with many different boxes, ranging from Easy to Insane. Some of these boxes can be very CTFy and most are probably out of scope for the OSCP exam. There is a list compiled by TJ Null, which goes through some OSCP like boxes, I would suggest 90% of these be completed before attempting the exam. Hack The Box is arguably the best when it comes to priv esc as there is lots of variety. To do the boxes on the list you will have to buy HTB VIP, which is around £10 a month.

<img src="/assets/images/oscp_list.jpg"/>

### Ippsec Videos

<a href="https://www.youtube.com/channel/UCa6eh7gCkpPo5XXUDfygQQA">IppSec's youtube channel</a>

I think this is one of the most crucial things you can do, watch IppSec's videos in your free time, even boxes that would be considered too hard for OSCP. You could learn something from a harder box and apply it during your exam. You'll also be able see how he enumerates each port/service and add that to your methodology. I would suggest first attempting the boxes before watching the IppSec tutorials, especially for the more OSCP-esque boxes. Best of all it's free!

### TryHackMe

<a href="https://tryhackme.com/">TryHackMe</a>

TryHackMe has a lot of beginner friendly boxes, and a dedicated "OSCP Learning Path", I feel the boxes in this path really helped me learn new things. The site has a different style to most, where you have to answer certain questions in order to complete the box as well as submitting flags. I feel like this can be a bit annoying as some of the questions are a bit weird. All in all though, I feel like this is a great resource. The membership cost just under £8 a month. 

### PWK

<a href="https://www.offensive-security.com/pwk-oscp/">PWK</a>

NOTE: I took the old version of the PWK, they updated the course just after I bought it, so I will be talking about the old version and not the new. 

PWK is the course for OSCP from Offsensive Security. In the end I only completed around 20 boxes, 2 of which are part of the "Big Four". Some of the machines in the course were very old so had multiple ways to get shells, which made it hard to differentiate to what the intended route was. However, if that method gets you a shell then I guess it's good enough. I tried to avoid metasploit, but I did end up using it on a few boxes. 

I didn't end up submitting the lab report and exercises as there were just so many exercises. However, I would probably suggest doing so if you have the time, those 5 extra points could be crucial. 

### Tib3rius' Privelege Escalation courses

<ul>
  <li><a href="https://www.udemy.com/course/linux-privilege-escalation/?referralCode=0B0B7AA1E52B4B7F4C06">Linux Privilege Escalation</a></li>
  <li><a href="https://www.udemy.com/course/windows-privilege-escalation/?referralCode=9A533B41ECB74227E574">Windows Privilege Escalation</a></li>
</ul>

These courses are concise and explain the basics of privielege escalation for both Linux and Windows, it was great to have everything you need in one place instead of various different articles spread across the internet. Would definitely recommend these.

# Tools

There are various different tools that can be used to assist you, I will highlight the top 3 for me, but leave it to you to research tools you feel like would help you. 

### AutoRecon

<a href="https://github.com/Tib3rius/AutoRecon">AutoRecon</a>

AutoRecon does all the basic recon for you automatically in the background and can save you a lot of time from doing it yourself.

### Linux Smart Enumeration

<a href="https://github.com/diego-treitos/linux-smart-enumeration">LSE</a>

LSE is a linux privilege escalation script which will help you find basic misconfigurations or things that could be suspicious and help you get root. 

### PEAS

<a href="https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite">PEAS</a>

PEAS are a set of linux and windows privilege escalation scripts. Adding these to your arsenal will help make escalating your privileges that little bit easier




