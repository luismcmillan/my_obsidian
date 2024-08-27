[[EC2 - Elastic Compute Cloud]]

```Shell
ssh -i "my_web_server_connection.pem" ec2-user@ec2-18-184-117-30.eu-central-1.compute.amazonaws.com
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@         WARNING: UNPROTECTED PRIVATE KEY FILE!          @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
Permissions 0644 for 'my_web_server_connection.pem' are too open.
It is required that your private key files are NOT accessible by others.
This private key will be ignored.
Load key "my_web_server_connection.pem": bad permissions
ec2-user@ec2-18-184-117-30.eu-central-1.compute.amazonaws.com: Permission denied (publickey,gssapi-keyex,gssapi-with-mic).
```

Lösung:

Der Fehler tritt auf, weil die Berechtigungen für deine private Schlüsseldatei (`my_web_server_connection.pem`) zu offen sind. SSH erwartet, dass private Schlüsseldateien nur für den Besitzer lesbar sind, um die Sicherheit zu gewährleisten.

Um das Problem zu beheben, musst du die Berechtigungen für die Schlüsseldatei ändern. Hier ist, was du tun kannst:
```Shell
chmod 600 my_web_server_connection.pem
```