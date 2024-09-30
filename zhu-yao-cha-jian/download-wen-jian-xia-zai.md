---
description: 下载文件到serverdata\Download\file
---

# Download 文件下载

## 安装

* 见快速开始
* 首次运行将在`serverdata`下生成`Download`文件夹

## 配置信息

<details>

<summary><code>serverdata\Download\config.json</code>文件</summary>

```json
{
    "group_enable":false,
    "private_enable":true
}
```

</details>

<details>

<summary>面板</summary>



</details>

<table><thead><tr><th width="189">参数</th><th width="93">默认值</th><th width="109">值可为</th><th>说明</th></tr></thead><tbody><tr><td>group_enable</td><td>false</td><td>false|true</td><td>群聊触发 false不启用</td></tr><tr><td>private_enable</td><td>true</td><td>false|true</td><td>私聊触发 true启用</td></tr></tbody></table>

## 使用

### 权限

> <mark style="color:yellow;">管理</mark>

### 触发

<table><thead><tr><th width="220">命令</th><th>说明</th></tr></thead><tbody><tr><td>下载 &#x3C;<mark style="color:blue;">链接</mark>> &#x3C;<mark style="color:purple;">文件名</mark>></td><td><mark style="color:blue;">链接</mark>为直链 <mark style="color:purple;">文件名</mark>为保存的文件及格式</td></tr><tr><td>DL &#x3C;<mark style="color:blue;">链接</mark>> &#x3C;<mark style="color:purple;">文件名</mark>></td><td><mark style="color:blue;">链接</mark>为直链 <mark style="color:purple;">文件名</mark>为保存的文件及格式</td></tr></tbody></table>

<details>

<summary> 发送<code>下载 https://www.itdog.cn/frame/images/logo_2023.png logo.png</code></summary>

完成, 请核对大小: 0.01MB

</details>

<details>

<summary> 发送<code>DL https://www.itdog.cn/frame/images/logo_2023.png logo.png</code></summary>

完成, 请核对大小: 0.01MB

</details>

### 说明

命令间使用 空格分隔参数

完成不一定代表成功下载，请核对文件大小
