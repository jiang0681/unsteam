# unsteam
该教程仅供项目交流使用，无不良引导，旨在说明如何绕过steam启动steam上的游戏，以将游戏文件拷贝带到其他电脑上能无障碍启动。  

下面先简单分个类。   

## 一、可以直接启动的  
找到：
    
    \Steam安装目录\steamapps\common\游戏A名称\
文件夹，双击里面的游戏A.exe文件，可以在steam未启动的状态下直接启动游戏A。  

适用游戏：桐叶的宝石心，等。  

这种就是没验证的游戏，可以直接拷贝带走。

## 二、Steamless剥壳  
下载Steamless的最新Releases并解压，得到Steamless程序。  
![image](https://github.com/user-attachments/assets/2a26f232-c9e3-4b75-a90d-07988f148a5e)  

原仓库下载地址：  

    https://github.com/atom0s/Steamless/releases/latest
备份仓库下载地址：

    https://github.com/jiang0681/unsteam/releases/download/paks/Steamless.v3.1.0.5.-.by.atom0s.zip
双击steamless.exe应用程序，导入你想要剥壳的游戏B.exe文件(以Miside Demo举例)  
![image](https://github.com/user-attachments/assets/ac08f9b8-fa2e-438d-a542-86acb097e02c)  

点击Unpack File即可得到剥壳后的游戏B_unpacked.exe，双击它即可直接启动游戏B。  

适用游戏：东方冰之勇者记，等。  

附：Steamless的原仓库地址：  

    https://github.com/atom0s/Steamless

## 三、steamclient_loader套壳  
下载steamclient_loader并解压，得到下列文件：  
![image](https://github.com/user-attachments/assets/f3d947ed-df63-4930-a0eb-9559fe7dff83)  

下载地址：  

    https://github.com/jiang0681/unsteam/releases/download/paks/steamclient_loader.zip
记事本打开ColdClientLoader.ini；  

填写AppId，在steam商店页面找得到；  

填写Exe=游戏启动程序名，程序在"\Steam安装目录\steamapps\common\游戏C名称\"里；  

这里用双影奇境演示一遍：  
![image](https://github.com/user-attachments/assets/831b8449-5117-4521-93db-42d656f2837c)  

保存ini文件，双击steamclient_loader.exe即可运行游戏C。   

适用游戏：大部分steam游戏。  

附：goldberg_emulator启动器原仓库地址：  
    
    https://gitlab.com/Mr_Goldberg/goldberg_emulator
    
steamclient_loader.exe即来源于此。  

## 四、Steamless剥壳后运行不了，再用steamclient_loader套壳后可以运行  

同"三、"，Exe=填写Steamless剥壳后的游戏启动程序名。  

适用游戏：NieR: Automata，AIR重制版，等。  

## 五、GSE进阶
用GSE提供的steam_api64.dll替换掉原来的dll，双击原来的exe有可能可以直接启动。  

文件在“三、”的附加链接里。  
## 六、上述都不行的，放弃。  

  
# 一般流程  
#### 1、直接双击试试。  
#### 2、替换steam_api64.dll试试
#### 3、如果不行，用Steamless剥壳。  
##### 2.a、Steamless剥壳提示失败(有红字)，进4、  
##### 2.b、Steamless剥壳成功，但直接双击游戏运行报错，进4、   
#### 4、用steamclient_loader套壳
