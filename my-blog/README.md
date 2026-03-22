# 我的博客

一个简洁的静态博客，基于纯 HTML/CSS/JavaScript，可直接部署到 GitHub Pages。

## 快速开始

### 1. 创建 GitHub 仓库

1. 访问 [GitHub](https://github.com) 并登录
2. 点击右上角 **+** → **New repository**
3. 仓库名填写：`yourusername.github.io`（把 `yourusername` 换成你的 GitHub 用户名）
4. 选择 **Public**
5. 点击 **Create repository**

### 2. 上传博客文件

把 `my-blog` 文件夹里的所有内容上传到仓库：

```bash
# 如果你安装了 Git
cd e:\code\my-blog
git init
git add .
git commit -m "Initial blog"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

或者直接在 GitHub 网页上点击 **Add file** → **Upload files**，然后把文件夹里的文件拖进去。

### 3. 访问你的博客

等待 1-2 分钟，然后访问：

```
https://yourusername.github.io
```

## 自定义博客

### 修改个人信息

编辑 `index.html`：
- 标题：`我的博客`
- 副标题：修改 `.subtitle` 里的文字
- 关于我：修改 `.about` 里的内容

### 添加新文章

1. 在 `posts` 文件夹里创建新的 HTML 文件
2. 参考 `posts/first-post.html` 的格式
3. 在 `index.html` 的 `posts` 数组里添加文章信息

### 修改样式

所有样式都在 `index.html` 的 `<style>` 标签里，可以直接修改颜色、字体等。

## 项目结构

```
my-blog/
├── index.html          # 首页
├── posts/
│   ├── first-post.html  # 文章示例
│   └── ...
└── README.md           # 说明文档
```

## 提示

- 图片放在 `images` 文件夹，引用时用相对路径 `images/xxx.jpg`
- 如果想用自定义域名，在仓库设置 → Pages → Custom domain
