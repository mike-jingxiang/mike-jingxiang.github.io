# Academic Homepage

这是一个可以直接用于 GitHub Pages 的静态学术主页模板，风格刻意保持为经济学者常见的极简个人主页：白底、蓝色链接、左侧个人信息、右侧论文与简介。

## 如何填写

1. 打开 `index.html`。
2. 替换 `Your Name`、`你的中文名`、职位、学校、邮箱和简介。
3. 把论文 PDF 放进 `papers/`，把 CV 放进 `cv/`。
4. 将论文链接改成实际文件名，例如 `papers/my-paper.pdf`。
5. 如需头像，把照片放入 `assets/profile.jpg`，然后把首页中的 `portrait` 占位块改为：

```html
<img class="portrait-img" src="assets/profile.jpg" alt="Your Name">
```

同时可在 `styles.css` 里加入：

```css
.portrait-img {
  width: 184px;
  aspect-ratio: 4 / 5;
  object-fit: cover;
  border: 1px solid var(--rule);
  margin-bottom: 24px;
}
```

## 部署到 GitHub Pages

1. 新建一个 GitHub 仓库，仓库名可以是 `你的用户名.github.io`。
2. 把这个文件夹里的所有文件上传到仓库根目录。
3. 在 GitHub 仓库设置里打开 Pages。
4. 选择 `main` 分支和根目录。
5. 等待几分钟后访问 `https://你的用户名.github.io/`。

如果之后绑定个人域名，可以再添加 `CNAME` 文件。
