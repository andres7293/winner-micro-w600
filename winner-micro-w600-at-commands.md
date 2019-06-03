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

# SDK gcc
```bash
#Instalar paquetes necesarios 
pacman -S arm-none-eabi-gcc
pacman -S arm-none-eabi-binutils
pacman -S arm-none-eabi-newlib
wget http://www.winnermicro.com/en/upload/1/editor/1553604753411.zip -O WM_SDK_W60X_G3.02.00_En.zip
unzip -d WM_SDK_W60X_G3.02.00_En.zip
cd WM_SDK_W60X_G3.02.00_En
cd Tools/GNU
chmod +x createimg.sh
cd ..
chmod +x makeimg
chmod +x makeimg_dbg
chmod +x makeimg_all
cd GNU
make V=s
```
