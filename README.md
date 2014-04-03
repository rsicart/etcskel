etcskel
=======

Service configurations and tests.

#  Postfix and Dovecot (IMAP only)

One smtp server (MTA) that sends and receives messages (MDA) using smtp.
A imap server to permit users read emails everywhere.

## 1. Install packages

    root@debian # apt-get update && apt-get install postfix dovecot-core dovecot-imapd

## 2. Setup files (config from postfix and dovecot site documentation)

	Replace example.com by your FQDN. Be sure that MX record for this domain is correctly set.

    /etc/postfix/main.cf
    /etc/postfix/master.cf
    /etc/dovecot/conf.d/10-auth.conf
    /etc/dovecot/conf.d/10-master.conf


-- 

R. Sicart
