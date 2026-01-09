# How-to-download-Git
How to download Git 入门级教程
1 下载
官方下载页面（跨平台）：https://git-scm.com/downloads
Windows 安装程序： https://git-scm.com/download/win
macOS 安装： https://git-scm.com/download/mac
Linux 安装说明： https://git-scm.com/download/linux
若想要图形客户端（可选）：GitHub Desktop — https://desktop.github.com/
快速安装命令示例

macOS（Homebrew）:
brew install git
或安装 Xcode 命令行工具： xcode-select --install
Ubuntu / Debian:
sudo apt update
sudo apt install git
Fedora:
sudo dnf install git
Arch Linux:
sudo pacman -S git
Windows：
下载上面的 Windows 安装程序并运行安装向导
安装后使用cmd或者集成终端验证：

git --version

<img width="562" height="113" alt="屏幕截图 2026-01-09 201435" src="https://github.com/user-attachments/assets/9b3a743d-d5d2-4621-a750-a16fe5f70486" />

2 继续在终端操作
设置自己的姓名等
 git config --global user.name "你的名字your name"
  git config --global user.email "你的邮箱your email"
  <img width="702" height="52" alt="屏幕截图 2026-01-09 202601" src="https://github.com/user-attachments/assets/49513621-bc0b-44f8-9257-51834e76cd36" />
3.分享文件的初始化
打开vscode

  <img width="1028" height="577" alt="屏幕截图 2026-01-09 203950" src="https://github.com/user-attachments/assets/3fd17a4d-22ef-4b18-bca5-eb7b7cdb1e46" />
点击打开文件
<img width="1028" height="577" alt="屏幕截图 2026-01-09 203950" src="https://github.com/user-attachments/assets/db19a276-e1e9-4a75-b6c5-9751df111845" />
找到自己需要上传的目标文件夹（我以mra7a_ws为例）
<img width="997" height="647" alt="屏幕截图 2026-01-09 205020" src="https://github.com/user-attachments/assets/bea43b89-ffa6-45fb-aa0d-ec786ad773d0" />

Ctrl+`(esc下面按键)打开终端
<img width="1407" height="594" alt="屏幕截图 2026-01-09 205406" src="https://github.com/user-attachments/assets/9bbd68d4-a5f0-462b-af6b-7539f109eea1" />


4.开始生成分享github内容
在上一步打开的终端进行get初始化
git init
<img width="685" height="156" alt="屏幕截图 2026-01-09 210736" src="https://github.com/user-attachments/assets/dce1eaee-e67a-4c8e-97a4-299bcda8b499" />
将所有文件丢进去
git add .
输入完后会出现一堆的warning ,这是正常的，直到出现终端输入行为止
<img width="1219" height="83" alt="屏幕截图 2026-01-09 211229" src="https://github.com/user-attachments/assets/8e74b15b-5377-471d-a892-ced31fd0deea" />





