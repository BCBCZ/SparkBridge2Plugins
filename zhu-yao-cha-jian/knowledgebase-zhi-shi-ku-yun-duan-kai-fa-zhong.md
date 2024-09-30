---
description: 根据提问进行回答
---

# ⚠️ KnowledgeBase 知识库-云端\[开发中]

## 安装

* 见快速开始
* 首次运行将在`serverdata`下生成`KnowledgeBase`文件夹

## 配置信息

<details>

<summary><code>serverdata\KnowledgeBase\config.json</code>文件</summary>

```json
{
    "only_manage":true
}
```

</details>

<details>

<summary><code>serverdata\KnowledgeBase\api.json</code>文件</summary>

```json
{
    "api":"https://api.bcbcz.com/mc/KnowledgeBase/?ask=",
    "apit":"https://api.bcbcz.com/mc/KnowledgeBase/?ask="
}
```

</details>

<details>

<summary>面板</summary>



</details>

<table><thead><tr><th width="189">参数</th><th width="93">默认值</th><th width="109">值可为</th><th>说明</th></tr></thead><tbody><tr><td>only_manage</td><td>true</td><td>false|true</td><td>仅管理员触发 true 是</td></tr></tbody></table>

| 参数   | 默认值                                          | 说明     |
| ---- | -------------------------------------------- | ------ |
| api  | https://api.bcbcz.com/mc/KnowledgeBase/?ask= | 请求地址   |
| apit | https://api.bcbcz.com/mc/KnowledgeBase/?ask= | 备用请求地址 |

## 使用

### 权限

> <mark style="color:yellow;">管理</mark>或<mark style="color:blue;">成员</mark>

### 触发

<table><thead><tr><th width="220">命令</th><th>说明</th></tr></thead><tbody><tr><td>KB &#x3C;<mark style="color:blue;">参数</mark>></td><td><mark style="color:blue;">参数</mark>为任意内容</td></tr></tbody></table>

<details>

<summary> 发送<code>KB 转发服务日志</code></summary>

日志为空

</details>

### 说明

命令间使用 空格分隔参数

## 云端搭建

### 待更新
