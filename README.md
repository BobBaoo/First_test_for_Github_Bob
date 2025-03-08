以下是将 Markdown 基本语法和 Git 基本命令整合到一个 Markdown 文档中的完整内容：

```markdown
# Markdown 与 Git 基本用法指南

## 1. Markdown 基本语法

### 1.1 标题
使用 `#` 表示标题，`#` 的数量表示标题的级别（1 到 6 级）。

```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

---

### 1.2 段落和换行
- 段落：段落之间需要空一行。
- 换行：在行尾添加两个空格，或者使用 `<br>` 标签。

```markdown
这是第一段。

这是第二段。  
这是同一段的第二行。
```

---

### 1.3 强调
- **加粗**：用 `**` 或 `__` 包裹文本。
- *斜体*：用 `*` 或 `_` 包裹文本。
- ~~删除线~~：用 `~~` 包裹文本。

```markdown
**加粗文本**  
__加粗文本__  

*斜体文本*  
_斜体文本_  

~~删除线文本~~
```

---

### 1.4 列表
#### 无序列表
使用 `-`、`*` 或 `+` 表示无序列表。

```markdown
- 项目 1
- 项目 2
  - 子项目 2.1
  - 子项目 2.2
```

#### 有序列表
使用数字加点表示有序列表。

```markdown
1. 第一项
2. 第二项
   1. 子项 2.1
   2. 子项 2.2
```

---

### 1.5 链接和图片
#### 链接
- 内联链接：`[文本](URL)`
- 引用链接：`[文本][id]`，然后在文档底部定义 `[id]: URL`

```markdown
[Google](https://www.google.com)  

[GitHub][1]  
[1]: https://www.github.com
```

#### 图片
- 内联图片：`![替代文本](图片URL)`
- 引用图片：`![替代文本][id]`，然后在文档底部定义 `[id]: 图片URL`

```markdown
![Markdown Logo](https://markdownlogo.com/logo.png)  

![GitHub Logo][2]  
[2]: https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png
```

---

### 1.6 代码
#### 行内代码
用 `` ` `` 包裹代码。

```markdown
这是 `行内代码` 示例。
```

#### 代码块
用 ``` ``` 包裹代码块，并指定语言（可选）。

````markdown
```python
def hello():
    print("Hello, Markdown!")
```
````

---

### 1.7 引用
使用 `>` 表示引用。

```markdown
> 这是一个引用。
>
> 这是引用的第二行。
```

---

### 1.8 分隔线
使用 `-`、`*` 或 `_` 至少三个字符表示分隔线。

```markdown
---
```

---

### 1.9 表格
使用 `|` 和 `-` 创建表格。

```markdown
| 列 1 | 列 2 | 列 3 |
| ---- | ---- | ---- |
| 数据 1 | 数据 2 | 数据 3 |
| 数据 4 | 数据 5 | 数据 6 |
```

---

### 1.10 任务列表
使用 `- [ ]` 表示未完成任务，`- [x]` 表示已完成任务。

```markdown
- [x] 完成任务 1
- [ ] 完成任务 2
```

---

## 2. Git 基本命令

### 2.1 初始化仓库
初始化一个新的 Git 仓库。

```bash
git init
```

---

### 2.2 克隆仓库
克隆一个远程仓库到本地。

```bash
git clone https://github.com/用户名/仓库名.git
```

---

### 2.3 添加文件到暂存区
将文件添加到暂存区。

```bash
git add 文件名
```

添加所有更改的文件：

```bash
git add .
```

---

### 2.4 提交更改
提交暂存区的更改到本地仓库。

```bash
git commit -m "提交信息"
```

---

### 2.5 查看状态
查看工作区和暂存区的状态。

```bash
git status
```

---

### 2.6 查看提交历史
查看提交历史记录。

```bash
git log
```

---

### 2.7 推送到远程仓库
将本地提交推送到远程仓库。

```bash
git push origin 分支名
```

---

### 2.8 拉取远程仓库更新
拉取远程仓库的最新更改。

```bash
git pull origin 分支名
```

---

### 2.9 创建分支
创建一个新的分支。

```bash
git branch 分支名
```

切换到新分支：

```bash
git checkout 分支名
```

---

### 2.10 合并分支
将指定分支合并到当前分支。

```bash
git merge 分支名
```

---

### 2.11 删除分支
删除本地分支。

```bash
git branch -d 分支名
```

强制删除未合并的分支：

```bash
git branch -D 分支名
```

---

### 2.12 查看远程仓库
查看远程仓库信息。

```bash
git remote -v
```

---

### 2.13 配置 Git
设置用户名和邮箱。

```bash
git config --global user.name "你的用户名"
git config --global user.email "你的邮箱"
```

查看配置：

```bash
git config --list
```

---

## 3. 示例：从本地创建仓库并推送到 GitHub

### 3.1 初始化本地仓库
```bash
mkdir my-repo
cd my-repo
git init
```

### 3.2 创建 Markdown 文件
```bash
touch README.md
```

编辑 `README.md` 文件，添加内容。

### 3.3 添加并提交文件
```bash
git add README.md
git commit -m "添加 README.md 文件"
```

### 3.4 链接远程仓库
```bash
git remote add origin https://github.com/用户名/my-repo.git
```

### 3.5 推送到 GitHub
```bash
git push -u origin main
```

---

通过以上内容，你可以快速掌握 Markdown 的基本语法和 Git 的基本命令！如果有其他问题，请随时告诉我。
```

---

### 使用方法
1. 将上述内容保存为一个 `.md` 文件（例如 `README.md`）。
2. 使用 Markdown 编辑器（如 VS Code、Typora）或 GitHub 预览效果。
3. 如果需要，可以将此文件推送到 GitHub 仓库中。
