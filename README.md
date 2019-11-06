correcthorse.postfix
=========

An ansible role for configuring postfix. This is a very basic role meant to configure postfix for sending mail from a web server.

Role Variables
--------------
| Variable			| Default			| Notes				|
| :---				| :---				| :---				|
| postfix_myhostname		| ""				| 				|
| postfix_mydomain		| ""				|				|
| postfix_myorigin		| ""				|				|
| postfix_relayhost		| ""				|				|
| postfix_ses_integration	| false				|				|
| postfix_use_sasl		| false				|				|
| postfix_use_tls		| false				|				|
| postfix_use_generic		| true				|				|
| postfix_sasl_username		| "user"			|				|
| postfix_sasl_password		| "password"			|				|
| postfix_inet_interfaces | "localhost" |     |

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: correcthorse.postfix }

License
-------

MIT

Author Information
------------------

* [Joshua Rusch](https://correct.horse/)