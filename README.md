
imapsync - Email IMAP tool for syncing, copying, migrating and archiving email mailboxes between two imap servers, one way, and without  duplicates.

Basic command to transfer emails from one server to another server using IMAP SYNC

```
imapsync --host1 Source server IP --user1 gill@domain.com --password1 "gillt8mail" --ssl1 --port1 993 --noauthmd5 --host2 Destination server IP --user2 gill@domain.com --password2 "gilt8email" --ssl2 --port2 993 --noauthmd5

```

| IMAP SYNC command Option  | Desciption|
---------|-----------
--host1  |  Source or "from" imap server
--port1  |  Port to connect on host1
--user1  |  User to login on host1
--host2  |  "Destination" imap server
--port2  |  Port to connect on host2
--user2  |  Password for the user2
--ssl1   |  Use a SSL connection on host1. On by default if possible
--ssl2   |  Use a SSL connection on host2. On by default if possible
--noauthmd5 | Don’t use MD5 authentification



