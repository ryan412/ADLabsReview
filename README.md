# Active Directory Labs/exams Review


If you know me, you probably know that I've taken a bunch of Active Directory Attacks Labs so far, and I've been asked to write a review several times. After passing the CRTE exam recently, I decided to finally write a review on multiple Active Directory Labs/Exams! Note that when I say Active Directory Labs, I actually mean it from an offensive perspective (i.e. a red teamer/attacker), not a defensive perspective. Furthermore, I’m only going to focus on the courses/exams that have a practical portion. Those that tests you with multiple choice questions such as CRTOP from IACRB will be ignored. 

# Whoami
I graduated from an elite university (Johns Hopkins University) with a master’s degree in Cybersecurity. I have a strong background in a lot of domains in cybersecurity, but I'm mainly focused in penetration testing and red teaming. I am currently a senior penetration testing and vulnerability assessment consultant at one of the biggest cybersecurity consultancy companies in Saudi Arabia where we offer consultancy to numerous clients between the public and private sector. I hold a number of penetration testing certificates such as:
* OSCE
* OSCP
* CRTE
* GPEN
* eCPTX
* GWAPT
* OSWP
* CREST CRT
* eCPPTv2
* ECSA (Practical)

Additionally, I hold a certificate in Purple Teaming:
* GDAT

My current rank in Hack The Box is Omniscient, which is only achievable after hacking 100% of the challenges at some point. More information about me can be found here: https://www.linkedin.com/in/rian-saaty-1a7700143/

# General Recommendation
As a general recommendation, it is nice to have at least OSCP OR eCPPT before jumping to Active Directory attacks because you will actually need to be good network pentester to finish most of the labs that I'll be mentioning. If you think you're good enough without those certificates, by all means, go ahead and start the labs! These labs are at least for junior pentesters, not for total noobs so please make sure not to waste your time & money if you know nothing about what I'm mentioning. Moreover, some knowledge about SQL, coding, network protocols, operating systems, and Active Directory is kind of assumed and somewhat necessary in most cases. You should obviously understand and know how to pivot through networks and use proxychains and other tools that you may need to use. Specifically, the use of Impacket for a lot of aspects in the lab is a must so if you haven't used it before, it may be a good start. The use of at least either BloodHound or PowerView is also a must. Antivirus evasion may be expected in some of the labs as well as other security constraints so be ready for that too! The reason I'm saying all this is that you actually need the "Try Harder" mentality for most of the labs that I'll be discussing here. In fact, most of them don't even come with a course!

# Introduction

Some of the courses/labs/exams that are related to Active Directory that I've done include the following:

**HackTheBox's Endgames:** 
* P.O.O
* Xen
* Hades

**HackTheBox's Pro Labs:**
* Offshore
* RastaLabs

**Elearn Security's Penetration Testing eXtreme**
* eLearnSecurity Certified Penetration Tester eXtreme certification (eCPTX)

**Pentester Academy's Windows Red Team Lab**
* Certified Red Team Expert (CRTE)

There are of course more AD environments that I've dealt with such as the private ones that I face in "real life" as a cybersecurity consultant as well as the small AD environments I face in some of Hack The Box's machines. (I will obviously not cover those because it will take forever). Also, note that this is by no means a comprehensive list of all AD labs/courses as there are much more red teaming/active directory labs/courses/exams out there. There are 2 in Hack The Box that I haven't tried yet (one Endgame & one Pro Lab), CRTP from Pentester Academy (beginner friendly), PACES from Pentester Academy, Red Team Ops from Zero Point Security, and a couple of Specter Ops courses that I've heard really good things about but still don't have time to try them. Once I do any of the labs I just mentioned, I'll keep updating this article so feel free to check it once in a while!

I'll be talking about most if not all of the labs without spoiling much and with some recommendations too! All of the labs contain a lot of knowledge and most of the things that you'll find in them can be seen in real life. In fact, I've seen a lot of them in real life! I will also compare prices, course content, ease of use, ease of reset/reset frequency, ease of support, & certain requirements before starting the labs, if any.

Note that I've taken some of them a long time ago so some portion of the review may be a bit rusty, but I'll do my best :)

To begin with, let's start with the Endgames. Endgames can't be normally accessed without achieving at least "Guru rank" in Hack The Box, which is only achievable after finishing at least 90% of the challenges in Hack The Box. This includes both machines and side CTF challenges. This can be a bit hard because Hack The Box keeps adding new machines and challenges every single week. However, once you're Guru, you're always going to be Guru even if you stopped doing any machine/challenge forever. The good thing is, once you reach Guru, ALL Endgame Labs will be FREE except for the ones that gets retired. I've done all of the Endgames before they expire. To make things clear, Hack The Box's active machines/labs/challenges have no writeups and it would be illegal to share their solutions with others UNTIL they expire. So far, the only Endgames that have expired are P.O.O. & Xen. The catch here is that WHEN something is expired in Hack The Box, you will be able to access it ONLY with VIP subscriptions even if you are Guru and above! Additionally, solutions will usually be available for VIP users OR when someone writes a writeup for it online :) Another good news (assuming that you haven't done Endgames before) is that with your VIP subscription, you will be able to access 2 Endgames at the same time!


# Endgame Professional Offensive Operations (P.O.O.):

I've completed P.O.O Endgame back in January 2019 when it was for Guru ranked users and above so here is what I remember so far from it:


**Price:** Comes with Hack The Box's VIP Subscription (£10 monthly) regardless of your rank. If you ask me, this is REALLY cheap!

**Ease of use:** Easy. You get an .ovpn file and you connect to it.

**Ease of reset:** Can be reset ONLY after 5 VIP users vote to reset it. This is actually good because if no one other than you want to reset, then you probably don't need a reset!

**Ease of support:** Community support only! Meaning that you'll have to reach out to people in the forum to ask for help if you get stuck OR in the discord channel. 

**Course:** Doesn't come with any course, it's just a lab so you need to either know what you're doing or have the Try Harder mentality!

**Goal:** "The goal is to compromise the perimeter host, escalate privileges and ultimately compromise the domain while collecting several flags along the way."

**Certificate:** N/A. You'll just get one badge once you're done.

**Exam:** N/A.

**Difficulty:** Intermediate

**Release Date:** March 2018.

**Retired:** June 2020.

The lab itself is small as it contains only 2 Windows machines. Not really "entry level" for Active Directory to be honest but it is good if you want to learn more about MSSQL Abuse and other AD attacks. It is worth mentioning that the lab contains more than just AD misconfiguration. It needs enumeration, abusing IIS vulnerabilities, fuzzing, MSSQL enumeration, SQL servers’ links abuse, abusing kerberoastable users, cracking hashes, and finally abusing service accounts to escalate privileges to system! Overall, a lot of work for those 2 machines! If you think you're ready, feel free to start once you purchase the VIP package from here: https://www.hackthebox.eu/home/endgame/view/1
Since it is a retired lab, there is an official writeup from Hack The Box for VIP users + others are allowed to do unofficial writeups without any issues. **SPOILER ALERT** Here is an example of a nice writeup of the lab: https://snowscan.io/htb-writeup-poo/#


# Endgame Xen:

I've completed Xen Endgame back in July 2019 when it was for Guru ranked users and above so here is what I remember so far from it:


**Price:** Comes with Hack The Box's VIP Subscription (£10 monthly) regardless of your rank. If you ask me, this is REALLY cheap!

**Ease of use:** Easy. You get an .ovpn file and you connect to it.

**Ease of reset:** Can be reset ONLY after 5 VIP users vote to reset it. This is actually good because if no one other than you want to reset, then you probably don't need a reset!

**Ease of support:** Community support only! Meaning that you'll have to reach out to people in the forum to ask for help if you got stuck OR in the discord channel. 

**Course:** Doesn't come with any course, it's just a lab so you need to either know what you're doing or have the Try Harder mentality!

**Goal:** "The goal is to gain a foothold on the internal network, escalate privileges and ultimately compromise the domain while collecting several flags along the way."

**Certificate:** N/A. You'll just get one badge once you're done.

**Exam:** N/A.

**Difficulty:** Intermediate

**Release Date:** June 2019.

**Retired:** June 2020.

Even though the lab is bigger than P.O.O, it only contains only 6 machines, so it is still considered small. Not really "entry level" for Active Directory to be honest but it is good if you want to learn more about Citrix, SMTP spoofing, credential based phishing, multiple privilege escalation techniques, Kerberoasting, hash cracking, token impersonation, wordlist generation, pivoting, sniffing, and bruteforcing. A LOT of things are happening here. Definitely not an easy lab but the good news is, there is already a writeup available for VIP Hack The Box users!

If you want to learn more about the lab feel free to check it on this URL: https://www.hackthebox.eu/home/endgame/view/2


# Endgame Hades:

I've completed Hades Endgame back in December 2019 so here is what I remember so far from it:


**Price:** Free with Guru Rank and above

**Ease of use:** Easy. You get an .ovpn file and you connect to it.

**Ease of reset:** Can be reset ONLY after 5 Guru ranked users vote to reset it. This is actually good because if no one other than you want to reset, then you probably don't need a reset!

**Ease of support:** Community support only! Meaning that you'll have to reach out to people in the forum to ask for help if you got stuck OR in the discord channel. 

**Course:** Doesn't come with any course, it's just a lab so you need to either know what you're doing or have the Try Harder mentality!

**Goal:** "The goal is to gain a foothold on the internal network, escalate privileges and ultimately compromise the domain while collecting several flags along the way."

**Certificate:** N/A. You'll just get one badge once you're done.

**Exam:** N/A.

**Difficulty:** Hard

**Release Date:** October 2019.

**Retired:** Still Active.

Even though this lab is small, only 3 machines, in my opinion, it is actually more difficult than some of the Pro Labs! It contains a lot of things ranging from web application exploitation to Active Directory misconfiguration abuse. This lab actually has very interesting attack vectors that are definitely applicable in real life environments. I can't talk much about the lab since it is still active. However, all I can say is that you need a lot of enumeration and that it is easier to switch to Windows in some parts :) It is doable from Linux as I've actually completed the lab with Kali only, but it just made my life much harder ><. Yes Impacket works just fine but it will be harder to do certain things in Linux and it would be as easy as "clicking" the mouse in Windows. At that time, I just hated Windows, so I wanted to spend more time doing it in Linux even though the author of the lab himself told me to do it in Windows and that he didn't test it with Linux. My only hint for this Endgame is to make sure to sync your clock with the machine!

If you want to learn more about the lab feel free to check it on this URL: https://www.hackthebox.eu/home/endgame/view/3


# Pro Labs: Offshore:

There is a new Endgame called RPG Endgame that will be online for Guru ranked and above starting from June 16th. More information about it can be found from the following URL: https://www.hackthebox.eu/home/endgame/view/4 Since I haven't really started it yet, I can't talk much about it. Now that I've covered the Endgames, I'll talk about the Pro Labs. Note that I've only completed 2/3 Pro Labs (Offshore & RastaLabs) so I can't say much about Pro Labs:Cybernetics but you can read more about it from the following URL: https://www.hackthebox.eu/home/labs/pro/view/3. The only thing I know about Cybernetics is that it includes Linux AD too, which is cool to be honest. Anyway, as the name suggests, these labs are targeting professionals, hence, "Pro Labs." However, in my opinion, Pro Lab: Offshore is actually beginner friendly. In fact, I ALWAYS advise people who are interested in Active Directory attacks to try it because it will expose them to a lot of Active Directory Attacks :) Even though I'm saying it is beginner friendly, you still need to know certain things such as what I have mentioned in the recommendation section above before you start! 


I've completed Pro Labs: Offshore back in November 2019. Also, it is worth noting that all Pro Labs including Offshore, are updated each quarter. That being said, Offshore has been updated TWICE since the time I took it. This means that my review may not be so accurate anymore, but it will be about right because based on my current completion percentage it seems that 85% of the lab still hasn't changed :)


**Price:** one time £70 setup fee + £20 monthly. Note that this is a separate fee, that you will need to pay even if you have VIP subscription. Additionally, you do NOT need any specific rank to attempt any of the Pro Labs.

**Ease of use:** Easy. You get an .ovpn file and you connect to it.

**Ease of reset:** The lab gets a reset automatically every day.

**Ease of support:** Community support only! Meaning that you'll have to reach out to people in the forum to ask for help if you got stuck OR in the discord channel. 

**Course:** Doesn't come with any course, it's just a lab so you need to either know what you're doing or have the Try Harder mentality!

**Goal:** "Players will have the opportunity to attack 17 hosts of various operating system types and versions to obtain 34 flags across a realistic Active Directory lab environment with various standalone challenges hidden throughout."

**Certificate:** Yes. You'll receive 4 badges once you're done + a certificate of completion with your name. 

**Exam:** N/A.

**Difficulty:** Intermediate

**Release Date:** September 2018.

**Retired:** Still active & updated every quarter!

As I said, In my opinion, this Pro Lab is actually beginner friendly, at least to a certain extent. There are 17 machines & 4 domains allowing you to be exposed to tons of techniques and Active Directory exploitations! You will have to gain foothold and pivot through the network and jump across trust boundaries to complete the lab. There is web application exploitation, tons of AD enumeration, local privilege escalation, and also some CTF challenges such as crypto challenges on the side. It is worth noting that in my opinion there is a 10% CTF component in this lab. However, the other 90% is actually VERY GOOD! I would highly recommend taking this lab even if you're still a junior pentester. Note that I was Metasploit & GUI heavy when I tried this lab, which helped me with pivoting between the 4 domains. You can probably use different C2s to do the lab or if you want you can do it without a C2 at all if you like to suffer :) If you're new to BloodHound, this lab will be a magnificent start as it will teach you how to use BloodHound! Of course, you can use PowerView here, AD Tools, or anything else you want to use! More about Offshore can be found in this URL from the lab's author: https://www.mrb3n.com/?p=551

If you think you're ready, feel free to purchase it from here:
https://www.hackthebox.eu/home/labs/pro/view/2


# Pro Labs: RastaLabs:

I've completed Pro Labs: RastaLabs back in February 2020. As with Offshore, RastaLabs is updated each quarter. That being said, RastaLabs has been updated ONCE so far since the time I took it. This means that my review may not be so accurate anymore, but it will be about right :)


**Price:** one time £70 setup fee + £20 monthly. Note that this is a separate fee, that you will need to pay even if you have VIP subscription. Additionally, you do NOT need any specific rank to attempt any of the Pro Labs.

**Ease of use:** Easy. You get an .ovpn file and you connect to it.

**Ease of reset:** The lab does NOT get a reset unless if there is a problem! The reason being is that RastaLabs relies on persistence!

**Ease of support:** RastaMouse is actually very active and if you need help, he'll guide you without spoiling anything. Other than that, community support is available too through forums and Discord!

**Course:** Doesn't come with any course, it's just a lab so you need to either know what you're doing or have the Try Harder mentality. Actually, in this case you'll CRY HARDER as this lab is actually pretty "hard."

**Goal:** "The goal of the lab is to reach Domain Admin and collect all the flags."

**Certificate:** Yes. You'll receive 4 badges once you're done + a certificate of completion.

**Exam:** N/A.

**Difficulty:** Hard

**Release Date:** ~ January 2018.

**Retired:** Still active & updated every quarter!

Unlike Pro Labs Offshore, RastaLabs is actually NOT beginner friendly. It is intense! You will not be able to easily use MetaSploit as the AV is actually very up to date and it will not like a lot of the tools that you would want to use. There is also AMSI in place and other mitigations. This means that you'll either start bypassing the AV OR use native Windows tools. I've decided to choose the 2nd option this time, which was painful. Additionally, there was not a lot of GUI possibility here too, and I wanted to stay away from it anyway to be as stealthy as possible. There are about 14 servers that can be compromised in the lab with only one domain. Even though it has only one domain, in my opinion, it is still harder than Offshore, which has 4 domains. The lab also focuses on maintaining persistence so it may not get a reset for weeks unless if something crashes. The problem with this is that your IP address may change during this time, resulting in a loss of your persistence. It is worth noting that there is a small CTF component in this lab as well such as PCAP and crypto. Some flags are in weird places too. The lab will require you to do tons of things such as phishing, password cracking, bruteforcing, password manipulation, wordlist creation, local privilege escalation, OSINT, persistence, Active Directory misconfiguration exploitation, and even exploit development, and not the easy kind! More information about the lab from the author can be found here: https://static1.squarespace.com/static/5be0924cfcf7fd1f8cd5dfb6/t/5be738704d7a9c5e1ee66103/1541879947370/RastaLabsInfo.pdf

If you think you're ready, feel free to purchase it from here:
https://www.hackthebox.eu/home/labs/pro/view/1


# Elearn Security's Penetration Testing eXtreme & eLearnSecurity Certified Penetration Testing eXtreme Certificate:

Now that I'm done talking about the Endgames & Pro Labs, let's start talking about Elearn Security's Penetration Testing eXtreme (eCPTX v1). I took the course and cleared the exam back in November 2019. It is worth noting that Elearn Security has just announced that they'll introduce a new version of the course! (not sure if they'll update the exam though but they will likely do that too!) That being said, this review is for the PTXv1, not for PTXv2! There is a webinar for new course on June 23rd and ELS will explain in it what will be different!

**Price:** There are 3 course plans that ranges between $1699-$1999 (Note that this may change when the new version is up!). However, you can choose to take the exam only at $400 without the course. You can check the different prices and plans based on your need from this URL: https://www.elearnsecurity.com/course/penetration_testing_extreme/enroll/ Note that ELS do some discount offers from time to time, especially in Black Friday and Cyber Monday! For example, there is a 25% discount going on right now!

**Ease of use:** Easy. You get an .ovpn file and you connect to it. There are really no AD labs that comes with the course, which is really annoying considering that you will face just that in the exam!

**Ease of reset:** You are alone in the environment so if something broke, you probably broke it. For the exam you get 4 resets every day, which sometimes may not be enough.

**Ease of support:** There is some level of support in the private forum.

**Course:** Yes! PDF & Videos (based on the plan you choose).

**Goal:** Take the exam and become eCPTX.

**Certificate:** Only once you pass the exam!

**Exam:** Yes. 48 hours practical exam + 24 hours report. The good thing about ELS is that they'll give you your 2nd attempt for free if you fail!

**Difficulty:** Intermediate

**Release Date:** 2017 but will be updated this month!

**Retired:** this version will be retired and replaced with the new version either this month or in July 2020!


Unfortunately, not having a decent Active Directory lab made this a very bad deal given the course's price. In fact, if you are a good network pentester & you've completed at least 75% of Pro Labs Offshore I can guarantee you that you'll pass the exam without looking at the course! I always advise anyone who asks me about taking eCPTX exam to take Pro Labs Offshore! Their course + the exam is actually MetaSploit heavy as with most of their courses and exams. The course itself, was kind of boring (at least half of it). However, the course talks about multiple social engineering methods including obfuscation and different payload creation, client-side attacks, and phishing techniques. They also talk about Active Directory and its usual misconfiguration and enumeration. Additionally, they explain how to bypass some security measurements such as AMSI, and PowerShell's constraint language mode. They also mention MSSQL (moving between SQL servers and enumerating them), Exchange, and WSUSS abuse. They also rely heavily on persistence in general. The very big disadvantage from my opinion is not having a lab and facing a real AD environment in the exam without actually being trained on one. Moreover, the exam itself is mostly network penetration testing with a small flavor of active directory. Not really what I was looking for when I took the exam, but it was a nice challenge after taking Pro Labs Offshore.



# Windows Red Team Lab & Certified Red Team Expert Certificate:

Now that I'm done talking about the eLS AD course, let's start talking about Pentester Academy's. Pentestar Academy in general has 3 AD courses/exams. CRTP, CRTE, and finally PACES. The first one is beginner friendly and I chose not to take it since I wanted something a bit harder. The last one has a lab with 7 forests so you can image how hard it will be LOL. As such, I've decided to take the one in the middle, CRTE. I took the course and cleared the exam in June 2020, so this was my most recent AD lab/exam.

**Price:** It ranges from $600-$1500 depending on the lab duration. However, they ALWAYS have discounts! For example, currently the prices range from $299-$699 (which is worth it every penny)! You can read more about the different options from the URL: https://www.pentesteracademy.com/redteamlab

**Ease of use:** Easy. You get an .ovpn file and you connect to it in the labs & in the exam. 

**Ease of reset:** The lab gets a reset every day. However, the exam doesn't get any reset & there is NO reset button! You will have to email them to reset and they are not available 24/7. Meaning that you may lose time from your exam if something gets messed up. Even worse, you will NOT know if something gets messed up, so you'll just have to guess. 

**Ease of support:** They are very friendly, and they'll help you through the lab if you got stuck. During the exam though, if you actually needed something (i.e. if something broke), they will reply only during office hours (it seems).

**Course:** Yes! PDF & Videos.

**Goal:** finish the lab & take the exam to become CRTE.

**Certificate:** Only once you pass the exam!

**Exam:** Yes. 48 hours practical exam including the report. Note that if you fail, you'll have to pay for the exam voucher ($99)

**Difficulty:** Hard

**Release Date:** July 2018

**Retired:** Nope


This lab was actually intense & fun at the same time. In other words, it is also not beginner friendly. There are 2 difficulty levels. The default is hard. However, I would highly recommend leaving it this way! The lab focuses on using Windows tools ONLY. You'll have a machine joined to the domain & a domain user account once you start. From there you'll have to escalate your privileges and reach domain admin on 3 domains! This include abusing different kind of Active Directory attacks & misconfiguration as well as some security constraints bypass such as AppLocker and PowerShell's constraint language mode. Additionally, there is phishing in the lab, which was interesting! The lab also focuses on SQL servers’ attacks and different kinds of trust abuse. The course itself is not that good because the lab has "experts" as its target audience, so you won't get much information from the course's content since they expect you to know it! However, the labs are GREAT! They include a lot of things that you'll have to do in order to complete it. Note that there is also about 10-15% CTF side challenges that includes crypto, reverse engineering, pcap analysis, etc. However, submitting all the flags wasn't really necessary. Meaning that you will be able to finish it without actually doing them. Also, the order of the flags may actually be misleading so you may want to be careful with this one even if they tell you otherwise! The most important thing to note is that this lab is Windows heavy. Meaning that you won't even use Linux to finish it! You'll use some Windows built in tools, Windows signed tools such as Sysinternals & PowerShell scripts to finish the lab. Of course, Bloodhound will help here too. Same thing goes with the exam. I actually needed something like this, and I enjoyed it a lot!

The exam was rough, and it was 48 hours that INCLUDES the report time. I can't talk much about the exam, but it consists of 8 machines, and to pass you'll have to compromise at least 3 machines with a good report. However, you may fail by doing that if they didn't like your report. The only way to make sure that you'll pass is to compromise the entire 8 machines! Without being able to reset the exam/boxes, things can be very hard and frustrating. I had an issue in the exam that needed a reset, and I couldn't do it myself. I spent time thinking that my methods were wrong while they were right! I emailed them and received an email back confirming that there is an issue after losing at least 6 hours! They were nice enough to offer an extension of 3 hours, but I ended up finishing the exam before my actual time finishes so didn't really need the extension.

If you are planning to do something more beginner friendly from Pentester Academy feel free to try CRTP. I've heard good things about it.


# Red Team Ops & Certified Red Team Operator:

**WILL UPDATE THIS SOON**

**Price:** It ranges from £399-£649 depending on the lab duration. In my opinion, one month is enough but to be safe you can take 2. The content is updated regularly so you may miss new things to try ;)

**Ease of use:** Easy. You get an .ovpn file and you connect to it in the labs & in the exam. 

**Ease of reset:** You can reboot any 1 machine once every hour & you need 6 votes for a revert of the entire lab. In the exam, you are entitled to only 1 reboot in the 48 hours & you don't have any option to revert!

**Ease of support:** As with RastaLabs, RastaMouse is actually very active and if you need help, he'll guide you without spoiling anything. Other than that, community support is available too through Slack!

**Course:** Yes! HTML & Videos. The reason is, the course gets updated regularly & you have LIFE TIME ACCESS to all the updates (Awesome!)

**Goal:** finish the lab & take the exam to become CRTO OR use the external route to take the exam without the course if you have OSCP (not recommended).

**Certificate:** You get a badge once you pass the exam & multiple badges during complention of the course

**Exam:** Yes. 48 hours practical exam without a report. Note that if you fail, you'll have to pay for a retake exam voucher (£99)

**Difficulty:** ?

**Release Date:** January 2020

**Retired:** Nope



As a final note, I'm actually planning to take more AD/Red Teaming labs in the future, so I'll keep updating this page once I finish a certain lab/exam/course.


I hope that you've enjoyed reading!
If you have any questions, comments, or concerns please feel free to reach me out on Twitter @ https://twitter.com/Ryan_412_/

