# How-to-download-GitHow to download Git 入门级教程

## 1 下载安装包
下载到本地一直点“next”就安装完成了
官方下载页面（跨平台）：https://git-scm.com/downloads  
Windows 安装程序： https://git-scm.com/download/win  
macOS 安装： https://git-scm.com/download/mac  
Linux 安装说明： https://git-scm.com/download/linux  
若想要图形客户端（可选）：GitHub Desktop — https://desktop.github.com/

快速安装命令示例  
macOS（Homebrew）:
```bash
brew install git
```
或安装 Xcode 命令行工具：
```bash
xcode-select --install
```
Ubuntu / Debian:
```bash
sudo apt update
sudo apt install git
```
Fedora:
```bash
sudo dnf install git
```
Arch Linux:
```bash
sudo pacman -S git
```
Windows：下载上面的 Windows 安装程序并运行安装向导

安装后使用cmd或者集成终端验证：
```bash
git --version
```

<img width="562" height="113" alt="屏幕截图 2026-01-09 201435" src="https://github.com/user-attachments/assets/9b3a743d-d5d2-4621-a750-a16fe5f70486" />

## 2 继续在终端操作设置自己的姓名等
```bash
git config --global user.name "你的名字your name"
git config --global user.email "你的邮箱your email"
```

<img width="702" height="52" alt="屏幕截图 2026-01-09 202601" src="https://github.com/user-attachments/assets/49513621-bc0b-44f8-9257-51834e76cd36" />

## 3.分享文件的初始化
打开vscode

<img width="1028" height="577" alt="屏幕截图 2026-01-09 203950" src="https://github.com/user-attachments/assets/3fd17a4d-22ef-4b18-bca5-eb7b7cdb1e46" />

点击打开文件

<img width="1028" height="577" alt="屏幕截图 2026-01-09 203950" src="https://github.com/user-attachments/assets/db19a276-e1e9-4a75-b6c5-9751df111845" />

找到自己需要上传的目标文件夹（我以mra7a_ws为例）

<img width="997" height="647" alt="屏幕截图 2026-01-09 205020" src="https://github.com/user-attachments/assets/bea43b89-ffa6-45fb-aa0d-ec786ad773d0" />

Ctrl+`(esc下面按键)打开终端

<img width="1407" height="594" alt="屏幕截图 2026-01-09 205406" src="https://github.com/user-attachments/assets/9bbd68d4-a5f0-462b-af6b-7539f109eea1" />

## 4.开始生成分享github内容
在上一步打开的终端进行get初始化
```bash
git init
```

将所有文件丢进去
```bash
git add .
```
输入完后会出现一堆的warning ,这是正常的，直到出现终端输入行为止

```bash
git commit -m "字符串备注（英文字符）"
```
生成create文件，等待出现终端输入行为止

<img width="654" height="151" alt="屏幕截图 2026-01-09 211640" src="https://github.com/user-attachments/assets/07a6b7e7-de5f-41db-ba5c-5bbfd0d2190e" />

## 5.开始导入到github
新建仓库登录github ，左上角点击新建

<img width="1888" height="166" alt="屏幕截图 2026-01-09 212708" src="https://github.com/user-attachments/assets/5efd493f-b01e-40b9-bc89-ff3a00414722" />

看图，以下4个步骤新建仓库

<img width="1920" height="1032" alt="新建仓库 和另外 4 个页面 - 个人 - Microsoft​ Edge 2026_1_9 21_28_55" src="https://github.com/user-attachments/assets/7496d2c1-90ef-40b7-b1ca-603b4355253f" />

打开仓库，复制你仓库的地址（重要）

<img width="1920" height="1032" alt="Learn-to-innovate-and-Surpass_Aubo-double-robot-arm_ Warehouse links that can be fed to the deepseek model 和另外 4 个页面 - 个人 - Microsoft​ Edge 2026_1_9 21_38_55" src="https://github.com/user-attachments/assets/0a5019c7-4169-4cf0-b05f-4608af950fda" />

```bash
git remote add origin 你的仓库网址
```
注意：第一次使用会弹出需要登录github账号的页面，请确保登录成功

<img width="1194" height="104" alt="欢迎 - mra7a_ws - Visual Studio Code  管理员  2026_1_9 22_09_16" src="https://github.com/user-attachments/assets/d753eefb-469a-47c4-b1a7-66a255bd6248" />

依次按行输入：
```bash
git branch -m maingit fetch origin git rebase origin/main（注意：这个代码可能出现error: The following untracked working tree files would be overwritten by merge:        .vscode/BROWSE.VC.DB     请输入以下代码解决：     # 删除文件rm .vscode/BROWSE.VC.DB# 或者删除整个.vscode目录（如果不需要，与上行代码二选一）rm -rf .vscode# 继续rebasegit rebase --continue）git push -u origin main
```

刷新仓库页面，成功

<img width="1920" height="1032" alt="Editing How-to-download-Git_README md at main · Learn-to-innovate-and-Surpass_How-to-download-Git 和另外 7 个页面 - 个人 - Microsoft​ Edge 2026_1_9 22_35_04" src="https://github.com/user-attachments/assets/adda1790-6343-42b8-b4c6-56ff474451f1" />
