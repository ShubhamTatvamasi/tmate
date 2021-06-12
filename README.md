# tmate

open crontab:
```bash
crontab -e
```

add the following line:
```
@reboot bash -c "tmate -F"
```

update the config `~/.tmate.conf`
```
set tmate-api-key "tmk-iuroiweuronmvxnoslkfd"
set tmate-session-name "session-name"
set tmate-authorized-keys "~/.ssh/authorized_keys"
```

