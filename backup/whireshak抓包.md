打开电脑，进入cmd

<img width="2394" height="1268" alt="Image" src="https://github.com/user-attachments/assets/23512338-7114-48b8-aca1-c2c4d14fba67" />

输入ip.config/all回车，记下电脑ipv4地址。

手机电脑连接同一WiFi，打开wireshak，点击WLAN，然后用手机给电脑发图片。

在输入框中输入ip.addr==+电脑的ipv4地址，查找流过电脑的包。

<img width="2014" height="1288" alt="Image" src="https://github.com/user-attachments/assets/1c92ef43-50e3-4145-85df-e417e25572fd" />

然后点击放大镜的图标，查找十六进制：FF D8 FF（JPG图片格式）

找到相应的包，右键选择追踪流TCP，以原始数据保存文件尾为.jpg

<img width="1858" height="1294" alt="Image" src="https://github.com/user-attachments/assets/1acc9289-ae6f-402b-a322-74c6d4ea6b77" />

winhex打开保存的文件，点击搜索，查找hex数值，输入FF。

<img width="1474" height="1078" alt="Image" src="https://github.com/user-attachments/assets/71e30593-e0c7-4c52-8145-573a01b6b5b8" />

找到FF D8 FF。删除前面的hex值，然后保存。

<img width="1482" height="1048" alt="Image" src="https://github.com/user-attachments/assets/92d2c127-8b56-4e4a-8bc4-b6a72c8ff289" />

打开刚保存文件，即可看到图片

<img width="1466" height="1036" alt="Image" src="https://github.com/user-attachments/assets/0b14d049-5ddc-456e-914b-c15a3735ec04" />