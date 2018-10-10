# CodePathWeek7
Assignment for week 7

Exploit #1 - WordPress <= 4.2.2 - Authenticated Stored Cross-Site Scripting (XSS)
<img src="Authenticated XSS.gif" width="800">
<br>
Explanation of exploit
<br>
<img src="Screen Shot 2018-10-10 at 6.32.58 PM.png" width="800">

Exploit #2 - WordPress  4.0-4.7.2 - Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds
<img src="Embedded YouTube XSS.gif" width="800">
Explanation of exploit: <br>
By using a youtube embed link such as 
[embed src='https://youtube.com/embed/12345\x3csvg onload=alert('haha you got haxored')\x3e'][/embed] Wordpress will read the \x3c and \x3e as '<' and '>' respectively which will allow the alert to be created. <br>
Exploit #3 - Large File upload XSS for WordPress 4.7.2
<img src="Large File upload XSS.gif" width="800">
Explanation of explout: <br>
By uploading a file that exceeds the max allowed file size that also has malicious Javascript source code such as "Dinosaurs secret life<img "src=x onerror=alert(1)">.png" (but without the inner quotes) the payload is executed by the server when the file is rejected from being uploaded as it gets displayed in the error message that appears to notify the user that the file is too large.
