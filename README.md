# wkhtmltopdf_on_centos
Install latest wkhtmltopdf on centos 7.
### This is configurations specially for knp_snappy


### Replace version number if needed
```sh
$ wget https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.4/wkhtmltox-0.12.4_linux-generic-amd64.tar.xz
```

### Untar and move
```sh
$ unxz wkhtmltox-0.12.4_linux-generic-amd64.tar.xz
$ tar -xvf wkhtmltox-0.12.4_linux-generic-amd64.tar
$ mv wkhtmltox/bin/* /usr/local/bin/
```

### And don't forget delete these
```sh
$ rm -f wkhtmltox-0.12.4_linux-generic-amd64.tar
$ rm -rf wkhtmltox
```
### Finally enjoy!
```sh
$ /usr/local/bin/wkhtmltopdf http://www.google.com google.pdf
```
