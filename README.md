# 第零步 准备工作
安装[Github Desktop](https://desktop.github.com/)。当然如果你对git命令足够熟悉的话，可以选择使用git命令行来进行操作。

- 首先你需要Fork本项目，请点击右上角的Fork按钮，将本项目Fork到你的仓库中。

- 之后你需要Clone你Fork的项目到本地，可以使用Github Desktop，也可以使用git命令行。
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
语法：
```shell
hugo new content talkType/talkType_talkNumber.language.md --kind talk_kind
```
其中，`hugo new content`会创造一个新的文档。之后的内容则指定题目以及文档的模版种类。
- `talkType`：不同类型的type对应不同文件夹。为了确保内容结构规整，请使用下面的路径：
    - 行业Talk - “**intalk**”
    - TechTalk - "**techtalk**"
    - OR Talk - "**ortalk**"
- `talkType_talkNumber.language.md`：题目的格式。
    - `talkType`：与上面相同，在"intalks"，“techtalks”，"ortalks“中三选一。
    - `talkNumber`：需要添加的talk的编号。公众号推送里会表明，或是在最近一次同类型talk的编号上加一即可。
    - `language`：根据需要，在"**zh**"中文，和"**en**"英文，两者中选一个。
- `talk_kind`：文档模版的类型
    - 文档模版类型的格式与上一条，题目的格式，类似；其命名方式为`language_talkType`。
    - 例如：如果需要制作一期OR Talk的中文内容，则选择`language`为中文`zh`，`talkType`为OR Talk`ortalks`，以此类推。

**示范例子**
    - 需要制作中英双语版本，内容为第23期Tech Talk。那么需要两条指令，分别创造中文和英文的内容：
    ```
    hugo new content techtalk/techtalk_23.zh.md --kind zh_techtalk
    hugo new content techtalk/techtalk_23.en.md --kind en_techtalk
    ```
    - 需要制作中英双语版本，内容为第5期In Talk。那么需要两条指令，分别创造中文和英文的内容：
    ```
    hugo new content intalk/intalk_5.zh.md --kind zh_intalk
    hugo new content intalk/intalk_5.en.md --kind en_intalk
    ```
    
# 第三步 填写Mardown文件
你可以在上一步创建的文档模版中找到详细的填写指南，包括语法指导。如果你对Markdown语法不熟悉的话，请参考[Cheatsheet](https://www.markdownguide.org/cheat-sheet/)。

# 第四步 运行Hugo
- 本地预览 如果你想先在本地预览网页效果，可以使用以下命令：
```shell
hugo --gc --minity server
```
点击localhost:1313即可查看效果，如果需要停止预览，可以使用Ctrl+C。

# 第五步 上传到GitHub
当你确认内容无误之后，就可以上传到**你的**GitHub仓库了。

你可以使用
```shell
git add .#添加所有文件
git commit -m "这里填写你备注的信息"#提交文件
git push#上传到GitHub
```
或者使用GitHub Desktop来进行操作。