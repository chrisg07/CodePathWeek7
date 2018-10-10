# CodePathWeek7
Assignment for week 7

Exploit #1 - WordPress <= 4.2.2 - Authenticated Stored Cross-Site Scripting (XSS)
<img src="Authenticated XSS.gif" width="400">
<br>
Explanation of exploit
<br>
<img src="Screen Shot 2018-10-10 at 6.32.58 PM.png" width="400">

Exploit #2 - WordPress  4.0-4.7.2 - Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds

Explanation of exploit: <br>
By using a youtube embed link such as 
[embed src='https://youtube.com/embed/12345\x3csvg onload=alert('haha you got haxored')\x3e'][/embed] Wordpress will read the \x3c and \x3e as '<' and '>' respectively which will allow the alert to be created.
Exploit #3
