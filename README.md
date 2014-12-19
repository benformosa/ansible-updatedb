## updatedb

[![Build Status](https://travis-ci.org/Oefenweb/ansible-updatedb.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-updatedb) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-updatedb-blue.svg)](https://galaxy.ansible.com/list#/roles/2463)

Manage updatedb Debian-like systems.

#### Requirements

None

#### Variables

 * `updatedb_prune_bind_mounts` [default: `true`]: Whether or not bind mounts are scanned
 * `updatedb_prunenames` [default: `[]`]: A list of directory names (without paths) which should not be scanned (e.g. .git .bzr .hg .svn)
 * `updatedb_prunepaths` [default: `[/tmp, /var/spool, /media, /home/.ecryptfs]`]: A list of path names of directories which should not be scanned
 * `updatedb_prunefs` [default: `[NFS, nfs, nfs4, rpc_pipefs, afs, binfmt_misc, proc, smbfs, autofs, iso9660, ncpfs, coda, devpts, ftpfs, devfs, mfs, shfs, sysfs, cifs, lustre_lite, tmpfs, usbfs, udf, fuse.glusterfs, fuse.sshfs, curlftpfs, ecryptfs, fusesmb, devtmpfs]`]: A list of file system types (as used in /etc/mtab) which should not be scanned

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
  - updatedb
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-updatedb/issues)!
