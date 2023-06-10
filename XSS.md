# Online School Fees System v1.0 has stored cross-site scripting

BUG_Author: zhangyf

Website source code address: https://www.sourcecodester.com/php/11708/online-school-fees-system.html

Vulnerability File: /paysystem/branch.php

POST parameter "branch" exists stored cross-site scripting vulnerability

Payload: branch=<script>alert(document.cookie)</script>&address=1&detail=2&id=&action=add&save=

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/1.png)

Payload will trigger when a user visits on http://localhost/paysystem/branch.php

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/2.png)



