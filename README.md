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
  -u, --user     Set user to create keytab for (default: walteste)
  -d, --domain   Set AD domain (Default: d.ethz.ch)
  -o, --output   Set output file (default: walteste.keytab)
  -h, --help     Displays this message
```
