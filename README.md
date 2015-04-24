# notes-facebook-watchman

## Ubuntu Config
```sh
# Get Value
cat /proc/sys/fs/inotify/max_user_watches
# Set Value
echo fs.inotify.max_user_watches=32768 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p

# Get Value
cat /proc/sys/fs/inotify/max_user_instances
# Set Value
echo fs.inotify.max_user_instances=256 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p
```
