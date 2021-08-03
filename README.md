# tmate

install tmate:
```bash
export TMATE_VERSION=2.4.0

wget https://github.com/tmate-io/tmate/releases/download/$TMATE_VERSION/tmate-$TMATE_VERSION-static-linux-amd64.tar.xz
tar -xf tmate-$TMATE_VERSION-static-linux-amd64.tar.xz
sudo mv tmate-$TMATE_VERSION-static-linux-amd64/tmate /usr/local/bin

# Clean up
rmdir tmate-$TMATE_VERSION-static-linux-amd64
rm tmate-$TMATE_VERSION-static-linux-amd64.tar.xz
```

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

