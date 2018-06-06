# SGIN.CN-V9.4.10-product-has-XSS-in-login-page

company name is sgin.cn
product is xiangyun platform
version is V9.4.10
[description]
An xiangyun platform V9.4.10 product has XSS via the login_url parameter to /login.php.
------------------------------------------
[Information]
This company has a common vulnerability,which is /login.php exist a xss.The payload can be constructed so that the attacker can obtain the user's cookie, causing the user to be backstage
------------------------------------------
[Vulnerability Type]
Cross Site Scripting (XSS)
------------------------------------------
[Vendor of Product]
http://www.sgin.cn/
------------------------------------------
[Affected Product Code Base]
xiangyun platform - V9.4.10
------------------------------------------
[Affected Component]
affected page is /login.php,such as"http://www.86ant.com/login.php";affected code is "login_url" in /login.php.
------------------------------------------
[Attack Type]
 Remote

 ------------------------------------------
[Attack Vectors]
open the page http://www.86ant.com/login.php
use hackbar or another tools change referer
input:     "><input name="haha" value="" onmouseover=alert(document.cookie)>//
then commit.
 ------------------------------------------
 
