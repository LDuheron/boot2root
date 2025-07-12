# boot2root
Boot2Root is a 42 Network project that challenges us to find various methods to gain root access to a server from a provided .iso image.

## Table of Contents
- [About](#about)
- [Usage](#Usage)
- [Solution one](#)

## About

**Boot2Root** is a 42 Network project that challenges us to find various methods to gain root access to a server from a provided .iso image.

## Usage

1. Create a VM with the .iso image provided by the subject.

## Solution

Arriving on the VM, our only clue is from the subject : “**There will be no visible IP address, and there’s a reason why…”**


1) it seems that we was booted with command
## exec login ## 
which causes the user to exit from the current shell (and thus prevents the new logged in user to return to the session of the caller). 
- https://www.computerhope.com/unix/ulogin.htm
in password "Echo" command is disabled to prevent revealing the password.
is it enabled during promt login ? checked - no

sites with informations about attacks
https://attack.mitre.org/#
https://owasp.org/www-project-top-ten/
https://www.cvedetails.com/