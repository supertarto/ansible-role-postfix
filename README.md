# Ansible Role Postfix
[![CI](https://github.com/supertarto/ansible-role-postfix/actions/workflows/ci.yml/badge.svg)](https://github.com/supertarto/ansible-role-postfix/actions/workflows/ci.yml)


Install and configure Postfix with Ansible. This role is tested only with Debian, and is very simplistic but it suits my needs.

## Requirements
None

## Tested plateform
* Debian 12 (Bookworm)
* Debian 13 (Trixie)

## Role variables
postfix_hostname let you define your mailname (your domain name, just after the "@"). I've only tested the smarthost, with a distant SMTP configuration.

```yml
postfix_hostname: "{{ ansible_fqdn }}"
postfix_main_mailer_type: "smarthost"
postfix_smtp: mysmtp
```


## License
GPL V3.0
