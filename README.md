# RevolutionPi Docker
[Kunbus Revolution Pi](https://revolution.kunbus.de/) Docker Image

Currently supports `vcgencmd`, `piSerial`, `revpi-factory-reset`, `ip` commands.

### Open issues
- renaming the hostname to 'RevPiXXXX' seems to be not possible in Docker
- systemd is not woking
  - causes shutdown command to not work -> even though it's actually a silly command to run inside a docker container
  - *SOLUTION:* to run systemd change the command that starts the container (pid1) to `/sbin/init`. Then systemd and shutdown commands will work
  