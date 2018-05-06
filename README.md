# i-MSCP - internet Multi Server Control Panel - FrontEnd

i-MSCP (internet Multi Server Control Panel) is a software easing shared
hosting environments management on Linux servers. It support various services
such as Apache2, ProFTPD, VsFTPd, Dovecot, Courier, Bind9... and can be easily
extended through plugins and/or event listener files.

i-MSCP was designed for professional Hosting Service Providers (HSPs), Internet
Service Providers (ISPs) and IT professionals.

## Official Site & Documentation

* [i-MSCP Site](https://i-mscp.net/)
* [i-MSCP Forums](https://i-mscp.net/index.php/BoardList/)
* [i-MSCP Documentation](https://wiki.i-mscp.net/)

## Development

For development, we use [docker-compose](https://docs.docker.com/compose/);
make sure you have both that and Docker installed on your machine.

Launch docker containers:

```console
$ docker-compose up -d
```

You can then browse to `http://localhost:8080`, and any changes you make in the
project will be reflected immediately.

## License

Unless otherwise stated all code is licensed under LGPL 2.1 and has the
following copyright:

```
    Copyright © 2010-2018 Laurent Declercq, i-MSCP™ | All Rights Reserved
```
