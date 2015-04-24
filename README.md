# notes-watchman

## Ubuntu Config
```sh
echo fs.inotify.max_user_watches=32768 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p

# To see current value
cat /proc/sys/fs/inotify/max_user_instances
# Set Value
echo fs.inotify.max_user_instances=256 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p
```
