# identity-to-hashcat
ASP.NET Identity (PBKDF2+HMAC-SHA256 or PBKDF2+HMAC-SHA1) to Hashcat format

Based on the original tool by @edernucci, modified to output the [John The Ripper](https://github.com/openwall/john) format as well.

Usage:
```
$ ./identity-to-hashcat.sh <hash>
```

Example:
```
$ ./id-to-hash.sh AGKcecrgyBNHkgjKqDlQPW7YlimD+VXPfpAx+gLSR0n1cOdIxFHaxKEF8SgAoaEtqQ==                


Hashcat: sha1:1000:Ypx5yuDIE0eSCMqoOVA9bg==:2JYpg/lVz36QMfoC0kdJ9XDnSMRR2sShBfEoAKGhLak= 

John: $pbkdf-sha1$1000$Ypx5yuDIE0eSCMqoOVA9bg$2JYpg/lVz36QMfoC0kdJ9XDnSMRR2sShBfEoAKGhLak 


```
