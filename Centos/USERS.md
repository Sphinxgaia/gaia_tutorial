# User manipulation centos

## Edit password

```bash
passwd username
```
or when already login
```
passwd
```

## Group add

### How to put username in groupname group

```bash
$ usermod -aG groupname username
```

### How to put username in sudoers group

```bash
$ usermod -aG wheel username
```
