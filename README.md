
imapsync - Email IMAP tool for syncing, copying, migrating and archiving email mailboxes between two imap servers, one way, and without  duplicates.

Basic command to transfer emails from one server to another server using IMAP SYNC

```
imapsync --host1 Source server IP --user1 gill@domain.com --password1 "gillt8mail" --ssl1 --port1 993 --noauthmd5 --host2 Destination server IP --user2 gill@domain.com --password2 "gilt8email" --ssl2 --port2 993 --noauthmd5

```

| IMAP SYNC command Option  | Description|
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
--tls1  | imapsync to use TLS on the source server, --tls2 will specify TLS on the destination server
--exclude| you can exclude a folder using the "–exclude" command
--folder | If you wanted to sync a single folder
--folderrec | If you needed to recursively include subfolders



#### IMAP SYNC command to use in office365 or exchange email server migration process.

```
imapsync --host1 imap.sourceserver.com --user1 tuttu@example.com --password1 '"Maxa!"' --sep1 / --prefix1 "" --host2 outlook.office365.com --user2 tuttu@example.com --password2 '"*11a50"' --ssl2 --regextrans2 's/^INBOX\.(.+)/$1/' --nolog --timeout 6000 --usecache --errorsmax 6000 --addheader
```

#### IMAP SYNC Manaull command latest

```
imapsync --host1 SOURCE_SERVER --user1 SOURCE_EMAIL --password1 "SOUCRE_PASSWORD" --sep1 / --host2 DESTINATION_SERVER --user2 DESTINATION_EMAIL --password2 "DESTINATION_PASSWORD" --nolog --timeout 900 --usecache --addheader
```
