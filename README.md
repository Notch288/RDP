(ALL COMMANDS ARE WRITTEN BY GW KANG)

pkg install gh -y && gh auth login -s codespace && gh cs create

cd /data/data/com.termux/files/usr/bin && touch startrdp && touch stoprdp

echo "gh cs ssh -c automatic-pancake-v6qj795x56j7hwr5p" >> startrdp && echo "gh cs stop -c automatic-pancake-v6qj795x56j7hwr5p" >> stoprdp && chmod +x * && cd

startrdp

sudo apt update && sudo apt upgrade -y && sudo apt install xfce4 -y && wget https://dl.google.com/linux/direct/chrome-remote-desktop_current_amd64.deb -P /tmp && sudo apt install --assume-yes /tmp/chrome-remote-desktop_current_amd64.deb
  
(ENTER THIRD CODE FROM CHROME REMOTE DESKTOP WEBSITE)

 /opt/google/chrome-remote-desktop/chrome-remote-desktop --stop && sudo apt install --assume-yes xfce4 desktop-base dbus-x11 xscreensaver
    
sudo bash -c 'echo "exec /etc/X11/Xsession /usr/bin/xfce4-session" > /etc/chrome-remote-desktop-session'

echo "export CHROME_REMOTE_DESKTOP_DEFAULT_DESKTOP_SIZES=1080x720,3840x2560" \
    >> ~/.profile
    
echo "/opt/google/chrome-remote-desktop/chrome-remote-desktop --start && /opt/google/chrome-remote-desktop/chrome-remote-desktop --start" >> ~/.bashrc
