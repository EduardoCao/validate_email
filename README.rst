参考资料：
1.如何验证 Email 地址：SMTP 协议入门教程 阮一峰 http://www.ruanyifeng.com/blog/2017/06/smtp-protocol.html?utm_source=tuicool&utm_medium=referral
2.【如何校验邮件地址的有效性】第三篇 ：原理二 木子耗2009 http://blog.csdn.net/u011628250/article/details/72909796

==============
Validate_email
==============

Validate_email is a package for Python that check if an email is valid, properly formatted and really exists.



INSTALLATION
============

First, you must do::

    pip install validate_email

Extra
------

For check the domain mx and verify email exits you must have the `pyDNS` package installed::

    pip install pyDNS


USAGE
=====

Basic usage::

    from validate_email import validate_email
    is_valid = validate_email('example@example.com')


Checking domain has SMTP Server
-------------------------------

Check if the host has SMTP Server::

    from validate_email import validate_email
    is_valid = validate_email('example@example.com',check_mx=True)


Verify email exists
-------------------

Check if the host has SMTP Server and the email really exists::

    from validate_email import validate_email
    is_valid = validate_email('example@example.com',verify=True)


TODOs and BUGS
==============
See: http://github.com/syrusakbary/validate_email/issues