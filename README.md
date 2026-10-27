# OC-Jenkins

A Bash script that installs Jenkins on an Ubuntu server.

## What it does

`install.sh`:

- Sets up proxy settings for apt and wget.
- Installs NTP.
- Adds the Jenkins Debian package repository and installs Jenkins.
- Logs each step to `/root/puppet.log`.

It also has helper functions for installing, removing and restarting
packages and services.

## Tech

- Bash on Ubuntu or Debian
- Jenkins

## Usage

Edit the proxy and email settings at the top of `install.sh`, then run
it as root:

```sh
sudo ./install.sh
```

## License

Licensed under the Apache License 2.0. See [LICENSE](LICENSE).
