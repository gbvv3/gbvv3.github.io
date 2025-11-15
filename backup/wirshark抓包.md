打开电脑，进入cmd

<img width="2286" height="864" alt="Image" src="https://github.com/user-attachments/assets/703b84bc-e71c-4205-ae93-5a967f18fcb8" />

输入ip.config/all回车，记下电脑ipv4地址。

手机电脑连接同一WiFi，打开wireshak，点击WLAN，然后用手机给电脑发图片。

在输入框中输入ip.addr==+电脑的ipv4地址，查找流过电脑的包。

<img width="1270" height="838" alt="Image" src="https://github.com/user-attachments/assets/71df8006-c1ee-49f3-a883-324ce9f7fbd0" />

然后点击放大镜的图标，查找十六进制：FF D8 FF（JPG图片格式）

找到相应的包，右键选择追踪流TCP，以原始数据保存文件尾为.jpg

<img width="1262" height="904" alt="Image" src="https://github.com/user-attachments/assets/aad90fad-8bfe-4fe7-8743-d6855faf9614" />

winhex打开保存的文件，点击搜索，查找hex数值，输入FF。

<img width="1176" height="860" alt="Image" src="https://github.com/user-attachments/assets/dd2fd33b-28d0-4469-b49e-b9e50a0803c8" />

找到FF D8 FF。删除前面的hex值，然后保存。

<img width="1252" height="888" alt="Image" src="https://github.com/user-attachments/assets/cdc6178b-d816-408c-8647-9b8b2a725503" />

打开刚保存文件，即可看到图片。

![Image](https://github.com/user-attachments/assets/1c5c3abc-caac-4119-9050-770391783e94)