---
description: 根据提问进行回答
---

# KnowledgeBaseLocal 知识库-本地

## 安装

* 见快速开始
* 首次运行将在`serverdata`下生成`KnowledgeBaseLocal`文件夹

## 配置信息

<details>

<summary><code>serverdata\KnowledgeBaseLocal\data.json</code>文件</summary>

```json
[
  {
    "mod": "精确",
    "ask": "菜单 menu Menu MENU",
    "answer": "没配置，建议看公告"
  }
]
```

</details>

<details>

<summary>面板</summary>



</details>

<table><thead><tr><th width="189">参数</th><th width="93">默认值</th><th width="109">值可为</th><th>说明</th></tr></thead><tbody><tr><td>mod</td><td>必填</td><td>精确|模糊</td><td>匹配模式</td></tr><tr><td>ask</td><td></td><td></td><td>问题可为多个 使用 空格分隔</td></tr><tr><td>answer</td><td>必填</td><td></td><td>答案</td></tr><tr><td><a data-footnote-ref href="#user-content-fn-1"><mark style="color:red;">asko</mark></a></td><td>仅[mod模糊]填</td><td></td><td>问题二 可为多个 使用 空格分隔</td></tr></tbody></table>

## 使用

### 权限

{% hint style="info" %}
<mark style="color:blue;">成员</mark>
{% endhint %}

### 触发

<table><thead><tr><th width="220">命令仅管理</th><th>说明</th></tr></thead><tbody><tr><td>KBL <mark style="color:blue;">add</mark> &#x3C;<mark style="color:purple;">问题</mark>> &#x3C;<mark style="color:orange;">答案</mark>></td><td><mark style="color:blue;">添加</mark> <mark style="color:purple;">问题</mark>可为多个 使用<code>.:</code>英.:分隔 <mark style="color:orange;">答案</mark></td></tr><tr><td>KBL <mark style="color:blue;">addv</mark> &#x3C;<mark style="color:purple;">问题</mark>> &#x3C;<mark style="color:orange;">答案</mark>> &#x3C;<mark style="color:red;">问题2</mark>></td><td><mark style="color:blue;">添加</mark> <mark style="color:purple;">问题</mark>可为多个 使用<code>.:</code>英.:分隔 <mark style="color:orange;">答案</mark> <mark style="color:red;">问题2</mark>可为多个 使用<code>.:</code>英.:分隔</td></tr><tr><td>KBL <mark style="color:blue;">delete</mark> &#x3C;<mark style="color:purple;">问题</mark>></td><td><mark style="color:blue;">删除</mark> <mark style="color:purple;">问题</mark></td></tr><tr><td>KBL <mark style="color:blue;">deleter</mark></td><td><mark style="color:blue;">删除</mark>没有被引用的资源</td></tr><tr><td>KBL <mark style="color:blue;">list</mark> &#x3C;<mark style="color:purple;">可选页码</mark>></td><td><mark style="color:blue;">列出</mark>问答 <mark style="color:purple;">页码</mark>  [<mark style="background-color:red;">没优化</mark>]</td></tr><tr><td>KBL <mark style="color:blue;">up</mark> &#x3C;<mark style="color:purple;">图片</mark>></td><td><mark style="color:blue;">上传</mark> <mark style="color:purple;">图片</mark></td></tr><tr><td>KBL <mark style="color:blue;">upv</mark></td><td><mark style="color:blue;">上传下一个视频</mark> [<mark style="color:yellow;">管理</mark>]</td></tr><tr><td>KBL <mark style="color:blue;">upi</mark></td><td><mark style="color:blue;">上传下一张图片</mark> [<mark style="color:yellow;">管理</mark>]</td></tr></tbody></table>

<details>

<summary>发送<code>KBL add 精确测试 这是个精确问题</code></summary>

<mark style="color:blue;">添加成功</mark>

发送`精确测试`

<mark style="color:blue;">这是个精确问题</mark>

成功添加`KBL add 精确1.:精确2 精确多词问题`

发送`精确1`或`精确2`

<mark style="color:blue;">精确多词问题</mark>

</details>

<details>

<summary>发送<code>KBL addv 模糊测试 这是个模糊问题</code></summary>

<mark style="color:blue;">添加成功</mark>

发送`阿巴模糊测试啦`

<mark style="color:blue;">这是个模糊问题</mark>

成功添加`KBL addv 模糊1.:模糊2 模糊多词问题`

发送`同人模糊1更新`或`同人模糊2更新`

<mark style="color:blue;">模糊多词问题</mark>

成功添加`KBL addv 模糊a.:模糊b 模糊多词二次问题 词1`

发送`上次模糊a没玩够词1啦`或`上次模糊b没玩够词1啦`

<mark style="color:blue;">模糊多词二次问题</mark>

成功添加`KBL addv w模糊.:x模糊 模糊多词二次多词问题 y词.:z词`

发送`欢乐w模糊港湾z词不好玩y词`或`欢乐模糊港湾z词不好玩y词`

<mark style="color:blue;">模糊多词二次多词问题</mark>



</details>

<details>

<summary>发送<code>KBL delete x模糊</code></summary>

<mark style="color:blue;">删除成功</mark>

</details>

<details>

<summary>发送<code>KBL deleter</code></summary>

<mark style="color:blue;">ok</mark>

</details>

<details>

<summary>发送<code>KBL list</code></summary>

<mark style="color:blue;">{"mod":"精确","ask":"精确1 精确2","answer":"精确多词问题"}, {"mod":"模糊","ask":"模糊1 模糊2","answer":"模糊多词问题"}, {"mod":"模糊","ask":"模糊a 模糊b","answer":"模糊多词二次问题","asko":"词1"}</mark>

</details>

<details>

<summary>发送<code>KBL up 图片</code></summary>

★ 上<mark style="color:blue;">传成功1B8CFA1DD40538F321384B385DD8D59B.jpg</mark>

</details>

<details>

<summary>发送<code>KBL upv</code></summary>

<mark style="color:blue;">控制台返回</mark><mark style="color:blue;">`上传下个视频 "yes"`</mark>

发送`视频`

`★`` `<mark style="color:blue;">`上传成功a8bd740ae90a2fa4f1bfdd8b918f2b24.mp4`</mark>

</details>

<details>

<summary> 发送<code>KBL upi</code></summary>

<mark style="color:blue;">控制台返回</mark> <mark style="color:blue;"></mark><mark style="color:blue;">`上传下一张图片 "yes"`</mark>

发送`图片`

★ 上传<mark style="color:blue;">成功A98A922F2196066C28823932DD6C63F7.jpg</mark>

</details>

### <mark style="background-color:red;">说明\[必看]</mark>

命令间使用 空格分隔参数，多个问题使用`.:`英.:分隔，答案中有非引用的`[`请使用`.&`英.&代替

答案可使用`[video,文件名][image,文件名]`引用视频|图片文件

<details>

<summary>引用举例   确保云端文件夹中有被引用文件</summary>

成功添加`KBL add 美图 这是一张图[image,xxx.jpg]哦`

发送`美图`

<mark style="color:blue;">这是一张图图片哦</mark>

成功添加`KBL add 视频 这是一个视频[video,xxx.mp4]哦`

<mark style="color:blue;">这是一个视频哦</mark>  \[视频不可嵌入文字中单独发送]

<mark style="color:blue;">视频</mark>

</details>

#### <mark style="color:red;">注意</mark>

如果已经添加了错误的问答请前往`serverdata\KnowledgeBaseLocal\data.json`中删除或修正

<details>

<summary>问题与答案与问题2 参数与参数首尾<mark style="color:red;">不可以</mark>是表情</summary>

`KBL`` `<mark style="color:blue;">`add`</mark> <mark style="color:purple;">`[表情]`</mark> <mark style="color:orange;">`[表情]a`</mark>  这个例子<mark style="color:purple;">问题</mark>与<mark style="color:orange;">答案</mark>表情相连 是<mark style="color:red;">错误</mark>的

`KBL`` `<mark style="color:blue;">`add`</mark> <mark style="color:purple;">`[表情]`</mark>` ``a`<mark style="color:orange;">`[表情]`</mark>  这个例子<mark style="color:purple;">问题</mark>与<mark style="color:orange;">答案</mark>表情不相连 是<mark style="color:green;">正确</mark>的



</details>

[^1]: 请看使用说明
