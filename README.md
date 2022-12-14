 # This Is Part Of The BT Wi-Fi Autologin Services Also Available For

 - Windows
 - Linux
 - Android (& Chromebook)
 
 ### Available Here:
 https://github.com/aidanmacgregor/BTWi-Fi_Autologin_-_OpenWrt_Linux_ChromeOS_Android_Macrodroid_Windows.EXE
 
 # ![2528830](https://user-images.githubusercontent.com/11254983/164993973-1b534096-84a8-4785-bf39-ea177eea4274.png) OpenWrt Autologin Service, LED & Theme<br/>

This is a shell script that is used to automatically log in to a BT Wi-Fi network as a service on an OpenWrt device. The script is designed to start automatically when the device is powered on and run continuously in the background. It includes several functions that are used to start, stop, and manage the service, as well as a loop that checks for internet connectivity and logs in to the BT Wi-Fi network if necessary.

The script defines several variables that are used to configure the behavior of the service, including the ACCOUNTTYPE, USERNAME, and PASSWORD variables, which are used to specify the user's account type and login credentials. These variables are read from the /etc/rc.local file, which is a script that is executed when the device starts up.

The script includes several functions, including the start function, which is used to start the service, and the stop function, which is used to stop the service. The start function starts three loops in the background, including the btwifi_loop, which checks for internet connectivity and logs in to the BT Wi-Fi network if necessary, the cleanlog_loop, which limits the size of the log file, and the tls_loop, which installs the TLS (Transport Layer Security) certificate if it is not already installed on the device. The stop function kills the three loops and removes the PID files that are used to track the processes.

The script also includes several optional variables, such as the LOGSIZE, PING1, PING2, PING3, and LOGPATH variables, which are used to customize the behavior of the service. For example, the LOGSIZE variable is used to specify the maximum size of the log file, and the PING1, PING2, and PING3 variables are used to specify the websites to ping to check for internet connectivity.

# Features:

 - No Treminal Commands (GUI Based)
 - Automatically Detect internet & OpenWRT Version to install libustream-mbedtls if needed
 - Logging
 - Log Size Limt
 - Theme & LED Service also availible

## Install The tar.gz Files Using LUCI (System > Backup / Flash Firmware)
	
![Install](https://user-images.githubusercontent.com/11254983/173888569-542fbbdd-c7c9-41cf-8411-1eceed69610c.JPG)	

## Autologin Service (System > Startup)
	
![Startup (3)](https://user-images.githubusercontent.com/11254983/173452552-d591d1c8-edd6-460b-b9bf-39509da5fda1.JPG)

## Add Your Account (System > Startup > Local Startup)
	
![Local Startup (3)](https://user-images.githubusercontent.com/11254983/173452553-e6a26dde-2d85-478a-9c94-22dde81a19fc.JPG)

## OpenWrt Downloads
    
[Login Service](https://github.com/aidanmacgregor/BTWi-Fi_Autologin_-_OpenWRT/releases)
    
[LED Service](https://github.com/aidanmacgregor/BTWi-Fi_Autologin_-_OpenWRT/tree/main/OpenWrt%20Themes%20%26%20LED%20Service/OpenWrt%20LED%20Service)
    
[Themes](https://github.com/aidanmacgregor/BTWi-Fi_Autologin_-_OpenWRT/tree/main/OpenWrt%20Themes%20%26%20LED%20Service/OpenWrt%20Theme)
