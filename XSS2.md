BUG_Author: zhangyf

Vulnerability File: /paysystem/datatable.php

GET parameter "doj" exists reflected cross-site scripting vulnerability

Payload: /paysystem/datatable.php?student=1&doj=<script>alert(document.cookie)</script>&type=feesearch

The js code is successfully executed and the cookie value is returned, which proves that there is a reflected cross-site scripting vulnerability.

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/4.png)
