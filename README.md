dsnapshot
=========
The dsnapshot script provides a high-level interface to the [Linux Logical
Volume Manager (LVM)][1]. It uses its block-level snapshot support to create
directory-level snapshots.

[1]: https://secure.wikimedia.org/wikipedia/en/wiki/Logical_Volume_Manager_%28Linux%29

Usage
-----
Create a new snapshot (returns a path/handle to the snapshot):

```
$ dsnapshot --create /srv/mysql/test/
/var/lib/dsnapshot/srv-fdf2e6dc/mysql/test/
```

Remove this snapshot:

```
$ dsnapshot --remove /var/lib/dsnapshot/srv-fdf2e6dc/mysql/test/
```

Todo
----
- add support for other backends like btrfs, freebsd etc.

Links
-----
http://benjamin-schweizer.de/dsnapshot.html
