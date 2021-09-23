# PremierSQL MiddleWare Server

Contains Archives for:
* Windows 32bit Academia Server Build
* Windows 64bit Release Candidate Client

## Server Installation

Unpack the PSQLMWSv16.ZIP into a folder, it only contains the Server EXE file.
Running PSQLMWS.EXE will generate the following folders:

* C:\Premier\
* C:\Premier\SQL\
* C:\Premier\SQL\Data\       (this is the root to all "DATABASES")
* C:\Premier\SQL\Log\
* C:\Premier\SQL\Whitelist\  (this is an IMPORTANT folder, see below);
* C:\Premier\SQL\Blocked\    (If you are developing your own client, and things do not work - check here for your IP!)

In Whitelist folder, you need to make 3 lined text files using the clients IP address.
![whitelist_example](https://user-images.githubusercontent.com/13199666/134448332-18541ad2-344c-43ac-8ef1-05a065203d63.png)

The content of the files is as follows:
LINE1: USER ID
LINE2: PASSWORD
LINE3: DESCRIPTION

So, initially if you have the server and client installed on the same machine, you want to make a 127.0.0.1 file.
With the contents:
OZZ NIXON
PASSWORD
LOCALHOST CLIENT

__Please Note__ Pressing ANY KEY while the PSQLMWS.EXE window has focus, is processed as a request to shutdown ASAP.
