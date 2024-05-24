# 第一步 安装Hugo
你可以选择命令行安装，也可以选择下载安装包安装。
```shell
choco install hugo-extended #for windows
brew install hugo #for mac
sudo snap install hugo #for Linux
```
完整的安装指南请参考： [Installing Hugo](https://www.gohugo.org/doc/overview/installing/)
> 别忘了把hugo.exe添加到环境变量PATH中

# 第二步 创建内容
```shell
hugo new xxx.md -k %TODO @amy20133511
```
# 第三步 填写Mardown文件
Markdown的语法请参考：[Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
# 第四步 运行Hugo
- 本地预览 如果你想先在本地预览网页效果，可以使用以下命令：
```shell
hugo server
```
点击localhost:1313即可查看效果，如果需要停止预览，可以使用Ctrl+C。
- 上传到GitHub Pages
如果你对Shell脚本比较熟悉，可以采用git add git commit git push的方式上传到GitHub即可完成部署。
如果你不熟悉Shell脚本，使用[Github Desktop](https://desktop.github.com/)也是一个不错的选择。
