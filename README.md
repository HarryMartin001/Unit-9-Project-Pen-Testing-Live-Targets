# Pen Testing Live Targets

Time spent: 6 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each color is vulnerable to only 2 of the 6 possible exploits. First discover which color has the specific vulnerability, then write a short description of how to exploit it, and finally demonstrate it using screenshots compiled into a GIF.

## Blue

Vulnerability #1: __________________
![sqlInjection](https://user-images.githubusercontent.com/111730072/200134023-92665f83-b667-47e7-a144-a600cdcf9489.gif)

Description:

<img src="blue-vuln1.gif">
The Attacker is Injects a sql command instead of the proper Salesperson's ID Number.
 Injected SQL Command:
%27%20OR%20SLEEP(5)=0--%27

## Green

Vulnerability #1: __________________
![UsernameEnumeration](https://user-images.githubusercontent.com/111730072/200134070-667f7cb5-e340-45e3-9f2a-c7aae3f6b1f6.gif)

Description:
As you can see from above, the Green Website has the Username Enumeration error where the failure to login message differs for the Username that exists vs doesn't exist.
 Using Chrome's debugging tool, I was able to see that the Developer assigns two different classes, failed and failure, to the error message depending on the login senerio.
 The "failure" class is applied an bold style in css while "failed" class doesn't. (Screen shots below)
<img src="green-vuln1.gif">
![failed](https://user-images.githubusercontent.com/111730072/200134112-0f481b03-05f6-41a4-9d72-8e0a553c7661.png)
![failure](https://user-images.githubusercontent.com/111730072/200134130-f8f94f7f-8b92-4e68-ac1e-a56e01d0c6a4.png)


## Red

Vulnerability #1: __________________
![GIF 2](https://user-images.githubusercontent.com/111730072/200134152-b54a69c8-2335-467c-a058-64e92a9d5d6f.gif)

Description:
![csrf](https://user-images.githubusercontent.com/111730072/200134194-760536d6-096d-436f-afd2-c540fe4f5527.gif)

<img src="red-vuln1.gif">


## Notes

no challenges during the work 
