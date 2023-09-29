# Some of the screens black but with the cursor working

```bash
journalctl -xe | grep -i "graphics\|display"
xrandr --auto
sudo dpkg --configure -a
```