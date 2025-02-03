## Ubuntu/Debian

- Real time watching

```
sudo apt update 
sudo apt install goaccess
```

## Fedora
```
$ yum install goaccess
```
## Arch Linux
```
$ pacman -S goaccess
```

## FreeBSD
```
$ pkg install sysutils/goaccess
```

## OpenBSD
```
$ pkg_add goaccess
```
## OpenSUSE
```
$ zypper ar -f obs://server:http http
$ zypper in goaccess
```

## Docker
```
$ tail -F access.log | docker run -p 7890:7890 --rm -i -e LANG=$LANG allinurl/goaccess -a -o html --log-format COMBINED --real-time-html - > report.html
```
https://goaccess.io/

