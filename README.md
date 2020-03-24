# fontCut

### 目的效果
通过python的fontTools插件，压缩剪切ttf、otf字体包，生成对应的css、woff文件<br />fontTools：<br />[github项目地址](https://github.com/fonttools/fonttools)<br />它还有很多功能，详情可以去了解了解。
### 场景
当时是需要在前端引入很多字体包，显示出不同的字体效果，而且文字是会动态变化的。直接引入所有字体包不现实，刚好当时在学习一点点python，就搜到了fontTools，刚好能达到我想要到效果。

- 事先准备好所有字体包的源文件
- 将此功能写成接口，前端动态的请求需要压缩的字体包和文字内容
- 生成对应的css、woff（压缩后，一般百来个中文就二三十kb）文件，返回给前端文件地址
- 前端代码引入并使用对应font-family即可
### 准备
目前代码用到了fontTools、time、pathlib、os、math等python库，需要安装入环境
```bash
pip install fonttools
```

### 使用
运行此文件即可，详细配置在代码注释
```bash
python3 fontToolMy.py
```
也是刚接触python，随意写写，满足了需求而已。乱写的乱写的

