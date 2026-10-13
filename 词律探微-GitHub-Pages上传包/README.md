# 词律探微：GitHub Pages 新手版

这是可以直接上传到 GitHub Pages 的静态演示原型，含 700 道公开题和 300 道验证题及答案。无需安装 Python、Node 或数据库。

## 上传并发布

建议新建一个演示仓库，避免覆盖参考仓库中的已有项目代码。

1. 登录 GitHub，右上角 **+ → New repository**。仓库名可填 `cilyutanwei-demo`，选择 **Public**，再点 **Create repository**。
2. 在新仓库中选择 **Add file → Upload files**。
3. 把本文件夹里的 `index.html`、`app.js`、`styles.css`、`benchmark.js`、`README.md` 五个文件上传到仓库根目录，然后点 **Commit changes**。
4. 打开仓库的 **Settings → Pages**。
5. 在 **Build and deployment** 中选择 **Deploy from a branch**；Branch 选 `main`，目录选 `/(root)`，点 **Save**。
6. 等部署完成后，在 **Settings → Pages** 页面点击站点网址。网址通常是：

   `https://你的GitHub用户名.github.io/cilyutanwei-demo/`

以后修改页面时重新上传并提交，GitHub Pages 会自动更新。

## 数据来源与结构

- [清词公开整理本](https://github.com/snowtraces/poetry-source)
- [宋词、元曲公开整理本](https://github.com/chinese-poetry/chinese-poetry)
- [GitHub 项目托管平台](https://github.com/)

题库以 `题号` 为主键，保留问题、答案、边界标签、判分规则和原始参考资料；新增 `source_ids` 连接到独立来源目录。页面中的参考链接可点击打开。

## 原型范围

页面演示声律解析、声情问答、论证辅助、校订建议、知识图谱和题库检索。问答是本地关键词检索，声律分析使用少量示例字表；尚未连接参考仓库中的 Python 服务或完整 58,000 余首词作语料库。

此包包含完整验证集题面和答案，并通过浏览器可读的静态文件加载。GitHub Pages 发布后，访客可下载这些文件。
