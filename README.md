# MLMOS
For creating a new SystemD unit file:

$ sudo touch /etc/systemd/system/foo-daemon.service
$ sudo chmod 664 /etc/systemd/system/foo-daemon.service

Basic structure of a unit file:
[Unit]
Description=Foo

[Service]
ExecStart=/usr/sbin/foo-daemon

[Install]
WantedBy=multi-user.target
