# Bro

#### Log locations

/nsm/bro/logs/ (Security Onion)


Get the originator and responder ip and port with a timestamp
```bro-cut -D %H:%M:%S ts id.orig_h id.orig_p id.resp_h id.resp_p```


Watch a bro log in realtime
```tail -n +1 -F conn.log | bro-cut ...```


Watch a bro log in realtime with a reverse grep
```tail -n +1 -F conn.log | stdbuf -o0 grep -v 192.168.1.2 | bro-cut ...```
