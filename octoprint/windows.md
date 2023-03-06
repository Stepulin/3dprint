### Managing services remotely

##### syntax

*sc \\X.X.X.X or dnsname **command** nameoftheservice*

Get the state/status of the service
```
sc \\10.1.97.10 query octoprint01
```

Stop the service
```
sc \\10.1.97.10 stop octoprint01
```

Start the service
```
sc \\10.1.97.10 start octoprint01
```
