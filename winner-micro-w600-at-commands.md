#AT Commands winer micro w600
```bash
#change to wifi sta mde
AT+WPRT=0
#Set SSID
AT+SSID="movistar5e"
#set wpa2 password
AT+KEY=1,0,"password"
#Run dhcp client to obtain ip address
AT+NIP=0
#start wifi association
AT+WJOIN
```

# SDK
```bash
wget http://www.winnermicro.com/en/upload/1/editor/1553604753411.zip -O WM_SDK_W60X_G3.02.00_En.zip
```
