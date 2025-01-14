




<h1 align="center">
  <br>
  <a href="https://play.google.com/store/apps/details?id=com.nex.tsports"><img src="https://github.com/byte-capsule/TSports-m3u8-Grabber/blob/main/images/TSports-logo.jpeg" alt="🔥 TSports 🔥" width="200"></a>
  <br>
  🔥 TSports 🔥
  <br>
</h1>

<h2 align="center">A Script to trigger the GitHub Actions every day to update the TSports App Channels M3U8 Link and Cookie </h2>

<p align="center">
  <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Made_With-Python_3.12%2B-blue"
         alt="Gitter">
  
  <a href="https://movielinks.pp.ua/live-tv/">
      <img src="https://img.shields.io/badge/Byte_Capsule-%E2%98%BC-green.svg">
  </a>
  <a href="https://movielinks.pp.ua/live-tv/">
    <img src="https://img.shields.io/badge/App-TSports_Live-red">
  </a>
  </a>
  <a href="https://movielinks.pp.ua/live-tv/"></a>
<a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fbyte-capsule%2FTSports-m3u8-Grabber&count_bg=%2379C83D&title_bg=%23555555&icon=mattermost.svg&icon_color=%23E7E7E7&title=Visitors+&edge_flat=false"/></a>
</p>

<h1 align="center">
 <a href="https://movielinks.pp.ua/live-tv/"><img src="https://github.com/byte-capsule/TSports-m3u8-Grabber/blob/main/images/TSports-banner.jpeg"></a>
</h1>

# 📒Introdicton 
* [TSports](https://movielinks.pp.ua/live-tv/) is a premium OTT platform that allows subscribers to watch live sports.By useing this Script you can watch all live sports for Free


# 💥Key Features

* All The Channel M3U8 Links and Cookies Are Updated Every 12 Hours 
* Premium Channels Are Also Working
* Contains Link With Headers (Host, Cookie)
* In JSON Format
* You Can Easily Use This on a Website or in an App for Restreaming TV Channels 



# 🕹️How To Use
**For Developers**
* 👉 **[Auto Updated Channels Json File](https://movielinks.pp.ua/live-tv/)**
* Use Get Request




```python
import requests
#Grab updated the M3U8 Link and Headers 
link="https://movielinks.pp.ua/live-tv/"
request=requests.get(link).json()

name=request["name"]
owner=request["owner"]
channels_amount=request["channels_amount"]
channels_data=request["channels"]
for channel in channels_data:
    link=channel["link"]
    headers=channel["headers"]
    print("✓ channel link :"+link)
    print("✓ channel Headers :",headers)
    



#Test The M3U8 Link and Cookie via Requesting TSports Server 
request_server=requests.get(link,headers=headers)
if request_server.status_code==200:
    print("😀 M3U8 Link and Cookies are Working.....")
    print("✓ Response From TSports Server : "+request_server.text)
else:
    print("🤧 M3U8 Link and Cookies are Not Working.....")
    print("✓ Response From TSports Server : "+request_server.text)
    




```

> **Note**
> I'm using Python 3.You can use other Languages.

# 🖥️Optput
>✓ channel link :https://movielinks.pp.ua/live-tv/
>✓ channel Headers : {'Cookie': 'Edge-Cache-Cookie=URLPrefix=aHR0cHM6Ly9saXZlLWNkbi50c3BvcnRzLmNvbS8:Expires=1702818302:KeyName=tsports-ed25519-01:Signature=ptxd7U8tSHlX6U4ImF-KojFqVq31ELgjeYl9rajJt_huoHfV86T9vLC0A79xPKbPa2fElmPe761MJW0fXEIMCw', 'Host': 'tsports.com', 'User-agent': 'https://movielinks.pp.ua/live-tv/ (Linux;Android 14)'}
>😀 M3U8 Link and Cookies are Working.....
>✓ Response From TSports Server : #EXTM3U
#EXT-X-VERSION:3
#EXT-X-STREAM-INF:BANDWIDTH=1482984,AVERAGE-BANDWIDTH=1482984,CODECS="avc1.640028,mp4a.40.2",PROGRAM-ID=1,RESOLUTION=1920x1080,FRAME-RATE=25.000
master_1080.m3u8
#EXT-X-STREAM-INF:BANDWIDTH=1278664,AVERAGE-BANDWIDTH=1278664,CODECS="avc1.64001f,mp4a.40.2",PROGRAM-ID=1,RESOLUTION=1280x720,FRAME-RATE=25.000
master_720.m3u8
#EXT-X-STREAM-INF:BANDWIDTH=1131528,AVERAGE-BANDWIDTH=1131528,CODECS="avc1.64001e,mp4a.40.2",PROGRAM-ID=1,RESOLUTION=854x480,FRAME-RATE=25.000
master_480.m3u8
#EXT-X-STREAM-INF:BANDWIDTH=780040,AVERAGE-BANDWIDTH=780040,CODECS="avc1.64001e,mp4a.40.2",PROGRAM-ID=1,RESOLUTION=640x360,FRAME-RATE=25.000
master_360.m3u8
#EXT-X-STREAM-INF:BANDWIDTH=624744,AVERAGE-BANDWIDTH=624744,CODECS="avc1.640015,mp4a.40.2",PROGRAM-ID=1,RESOLUTION=426x240,FRAME-RATE=25.000
master_240.m3u8
#EXT-X-STREAM-INF:BANDWIDTH=440808,AVERAGE-BANDWIDTH=440808,CODECS="avc1.64000c,mp4a.40.2",PROGRAM-ID=1,RESOLUTION=256x144,FRAME-RATE=25.000
master_144.m3u8
>
>[Program finished]
<h1 align="center">
 <a href="https://movielinks.pp.ua/live-tv/"><img src="https://github.com/byte-capsule/TSports-m3u8-Grabber/blob/main/images/IMG_20231216_170902.jpg"></a>
</h1>

# 🎬How To Play
**📱Android**
* Use NS (Network Stream Player) [Download](https://movielinks.pp.ua/live-tv/)
* Add This PlayList [Playlist Link](https://movielinks.pp.ua/live-tv/)
* 👆 Short Link : https://movielinks.pp.ua/
*  Enjoy 😊

**🖥️ Android TV**
* Use OTT Navigator [Download](https://movielinks.pp.ua/live-tv/)
* Add This PlayList [Playlist Link](https://movielinks.pp.ua/live-tv/)
* 👆 Short Link : https://movielinks.pp.ua/
*  Enjoy 😊

<h1 align="center">
 <a href="https://movielinks.pp.ua/live-tv/"><img src="https://github.com/byte-capsule/TSports-m3u8-Grabber/blob/main/images/Screenshot_2023-12-16-14-11-47-028_com.genuine.leone.jpg"></a>
</h1>
<h1 align="center">
 <a href="https://movielinks.pp.ua/live-tv/"><img src="https://github.com/byte-capsule/TSports-m3u8-Grabber/blob/main/images/Screenshot_2023-12-16-14-11-34-199_com.genuine.leone.jpg"></a>
</h1>

# 🚬Credits
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=100&color=FF2C10&background=31FF9400&width=400&lines=Made+By+Byte+Capsule)](https://git.io/typing-svg)

*🥰 Thanks:

- [Pydorid 3](https://movielinks.pp.ua/live-tv/)
- [Termux](https://movielinks.pp.ua/live-tv/)


# 📝Note
* The following code is for educational purposes only. It demonstrates how to authenticate and stream IPTV. Do not use it for any illegal or harmful activities. If the code affects the revenue of the IPTV owners, please let me  and I will delete it.
* Please give me proper credit if you share this content. Otherwise, I will take it down.
* The codes of the repo are encrypted to ensure security. Please refrain from trying to run or deploy them 
* Due to geo-restriction, the IPTV content is only available in Bangladesh.



# 💰Support

<a href="https://movielinks.pp.ua/live-tv/" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>




# ✉️Find Me on 

- [![Github](https://img.shields.io/badge/Github-Byte_Capsule-purple?style=for-the-badge&logo=github)](https://movielinks.pp.ua/live-tv/)

- [![Gmail](https://img.shields.io/badge/Gmail-Byte_Capsule-green?style=for-the-badge&logo=gmail)](mailto:shamimasraf299@gmail.com)

- [![Facebook](https://img.shields.io/badge/Facebook-Jeshan_Akand-blue?style=for-the-badge&logo=facebook)](https://t.me/code2shop)

- [![Messenger](https://img.shields.io/badge/Messenger-Jeshan_Akand-orange?style=for-the-badge&logo=messenger)](https://t.me/code2shop)

- [![Telegram](https://img.shields.io/badge/Telegram-Byte_Capsule-indigo?style=for-the-badge&logo=telegram)](https://t.me/code2shop)
