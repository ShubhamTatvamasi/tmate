# tmate

https://github.com/tmate-io/tmate/releases/download/2.4.0/tmate-2.4.0-static-linux-amd64.tar.xz

open crontab:
```bash
crontab -e
```

add the following line:
```
@reboot tmate -F
```

update the config `~/.tmate.conf` or `/root/.tmate.conf`
```
set tmate-api-key "tmk-iuroiweuronmvxnoslkfd"
set tmate-session-name "session-name"
set tmate-authorized-keys "~/.ssh/authorized_keys"
```

