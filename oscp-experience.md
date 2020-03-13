---
layout: default
---

# My OSCP experience
<hr />

I wanted to take OSCP to challenge myself and learn something new that has always interested me. When I began I didn't really know where to start, so hopefully this blog post will give people thinking of taking the exam some insight.

## My prior experience
<hr />

I have worked in InfoSec for around 3 years, most recently I have been working as a SOC Analyst, in the worst case scenrio, defending against the sort of attacks one might learn in their OSCP studies. I felt like doing OSCP would better help me notice malicious behavior, which in some ways it did. 

I held the CompTIA Network+, Security+ and CySA+ certifications prior to taking the OSCP. It would be fair to say I had a general idea of some of the attacks, but no clue how to perform one. Even the concepts of reverse shells were beyond me when I began. My linux experience wasn't too great, I could cd around directories and list files, but that was probably about it. 

## What did I use to study?
<hr />

I will go into some more detail about these resources after, but I used Virtual Hacking Labs, Hack the Box, TryHackMe, PWK, Ippsec Videos and Tib3rius' privelege escalation courses.

### Virtual Hacking Labs
<hr />

<a href="https://www.virtualhackinglabs.com/">Virtual Hacking Labs</a>

Virtual Hacking Labs was my intial exposure into the world of hacking. I bought the 3 month package, which comes with the 3 months in the labs and a courseware PDF. The courseware was very easy for me to follow and understand, it really holds your hand to make sure you understand what it is trying to teach. The machines in the labs have 3 ranks, Beginner, Advanced and Advanced+, so you can start easy and work your way up. There are slight nudges for the machines in the control panel, except for the Advanced+ where you are left on your own to try figure them out. I think the privilege escalation part of the course and labs could use some more variety, however I still think this is a great resource and part of the reason I passed.

### Hack The Box
<hr />

<a href="https://www.hackthebox.eu/">Hack The Box</a>

I'm sure the vast majority have already heard of Hack The Box. It's a great site with many different boxes, ranging from Easy to Insane. Some of these boxes can be very CTFy and most are probably out of scope for the OSCP exam. There is a list compiled by TJ Null, which goes through some OSCP like boxes, I would suggest 90% of these be completed before attempting the exam. Hack The Box is arguably the best when it comes to priv esc as there is lots of variety. To do the boxes on the list you will have to buy HTB VIP, which is around £10 a month.

<img src="/assets/images/oscp_list.jpg"/>

### Ippsec Videos
<hr />

<a href="https://www.youtube.com/channel/UCa6eh7gCkpPo5XXUDfygQQA">IppSec's youtube channel</a>

I think this is one of the most crucial things you can do, watch IppSec's videos in your free time, even boxes that would be considered too hard for OSCP. You could learn something from a harder box and apply it during your exam. You'll also be able see how he enumerates each port/service and add that to your methodology. I would suggest first attempting the boxes before watching the IppSec tutorials, especially for the more OSCP-esque boxes. Best of all it's free!

### TryHackMe
<hr />

<a href="https://tryhackme.com/">TryHackMe</a>

TryHackMe has a lot of beginner friendly boxes, and a dedicated "OSCP Learning Path", I feel the boxes in this path really helped me learn new things. The site has a different style to most, where you have to answer certain questions in order to complete the box as well as submitting flags. I feel like this can be a bit annoying as some of the questions are a bit weird. All in all though, I feel like this is a great resource. The membership cost just under £8 a month. 

### PWK
<hr />

<a href="https://www.offensive-security.com/pwk-oscp/">PWK</a>

NOTE: I took the old version of the PWK, they updated the course just after I bought it, so I will be talking about the old version and not the new. 

PWK is the course for OSCP from Offsensive Security. In the end I only completed around 20 boxes, 2 of which are part of the "Big Four". Some of the machines in the course were very old so had multiple ways to get shells, which made it hard to differentiate to what the intended route was. However, if that method gets you a shell then I guess it's good enough. I tried to avoid metasploit, but I did end up using it on a few boxes. 

I didn't end up submitting the lab report and exercises as there were just so many exercises. However, I would probably suggest doing so if you have the time, those 5 extra points could be crucial. 

### Tib3rius' Privelege Escalation courses
<hr />

<ul>
  <li><a href="https://www.udemy.com/course/linux-privilege-escalation/?referralCode=0B0B7AA1E52B4B7F4C06">Linux Privilege Escalation</a></li>
  <li><a href="https://www.udemy.com/course/windows-privilege-escalation/?referralCode=9A533B41ECB74227E574">Windows Privilege Escalation</a></li>
</ul>

These courses are concise and explain the basics of privielege escalation for both Linux and Windows, it was great to have everything you need in one place instead of various different articles spread across the internet. Would definitely recommend these.

## Tools
<hr />

There are various different tools that can be used to assist you, I will highlight the top 3 for me, but leave it to you to research tools you feel like would help you. 

### AutoRecon
<hr />

<a href="https://github.com/Tib3rius/AutoRecon">AutoRecon</a>

AutoRecon does all the basic recon for you automatically in the background and can save you a lot of time from doing it yourself.

### Linux Smart Enumeration
<hr />

<a href="https://github.com/diego-treitos/linux-smart-enumeration">LSE</a>

LSE is a linux privilege escalation script which will help you find basic misconfigurations or things that could be suspicious and help you get root. 

### PEAS
<hr />

<a href="https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite">PEAS</a>

PEAS are a set of linux and windows privilege escalation scripts. Adding these to your arsenal will help make escalating your privileges that little bit easier

## Exam day
<hr />

So the day to finally tackle the OSCP was here, I had booked it to start at 9AM, so it would just feel like a normal day. I connected to the proctoring software 15 minutes before the start time, which you recieve by email around 72 hours before the exam starts. I had an issue where my webcam wouldn't focus on my ID properly so I had to take a picture with my phone and display it on the screen for the proctor to see. After this, the proctoring ran smoothly in the backgroud and didn't cause me any more issues. 

The information you need for your boxes including the IPs are in the control panel, which you recieve by email when your exam starts. I would suggest copying this information out into notepad just to make it slightly easier to read. The control panel allows you to upload hashes and reset machines as well. 

I started AutoRecon running on the 4 other exam machines and started the buffer overflow. Within around an hour I had a working exploit and all my screenshots 

I then worked on a 20 pointer which I completed in around an hour, so I had 45 points and was feeling confident. I then had my first break for around 15 minutes to grab some more water and stretch my legs. 

I tackled the 10 pointer next, which took around 10-15 minutes to compromise, leaving me with 55 points. 

I looked through my other scans before deciding to go have some lunch. 

After my return I looked through the other 20 pointer, and figured out a way to get a shell after wondering why it wasn't working. Turns out I just don't know how to type properly. Always double check you're actually typing what your brain wants to type. I couldnt figure out the priv esc to this one within 30 minutes, so I moved on to last 25 point machine. Having a total of 65 points at around 4 hours in, I was feeling confident, but in the back of my mind hoping not doing the lab report wouldn't bite me in the arse. 

I managed to get a shell on the 25 pointer, after looking through my scans and doing a bit of further enumeration. That gave me a passing score of 77.5 points. I had another break for around 30 minutes before coming back to try tackle the final 2 priv escs. 

However, I couldn't figure them out within around 2 hours, so I started to create my report while thinking about what I could possibly do to escalate my privleges. I never did figure out what the priv esc was on either of them. 

I had my report pretty much completed by around 6 PM, but I thought I would sleep on it and wake up around 8 AM the following day just to make sure my tired mind hadn't missed anything crucial. 

For the report I used the 
<a href="https://github.com/whoisflynn/OSCP-Exam-Report-Template">WhoIsFlynn template</a>, just to make my report look that bit more professional. 

At around 9AM the following day, 24 hours after my exam began I sent my report off and the wait began. 

<img src="/assets/images/1weeklater.jpg"/>

After 1 horrible week of waiting, I finally recieved my results and I had passed! 

<img src="/assets/images/oscppass.png"/>





