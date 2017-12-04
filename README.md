user-keytab
===========

This utility creates a keytab file for an AD user account. The keytab 
keys are computed locally with the password of the user. The only
information queries from the active directory is the KVNO.

Usage
=====

```
user-keytab [--user user] [--domain domain] [--output file] [--help]

Options:
  -u, --user     Set user to create keytab for (default: $USER)
  -d, --domain   Set AD domain (Default: d.ethz.ch)
  -o, --output   Set output file (default: $USER.keytab)
  -h, --help     Displays this message
```

Requirements
============

user-keytab is written in perl. Install perl and the following modules from CPAN:
- Net::LDAPS
- Term::ReadKey
- File::Slurp
- Digest::HMAC_SHA1
- Crypt::Rijndael

On a CentOS/RHEL system you can install everything with the following command:

```
yum install -y perl perl-LDAP perl-TermReadKey perl-File-Slurp perl-Digest-HMAC perl-Crypt-Rijndael
```
