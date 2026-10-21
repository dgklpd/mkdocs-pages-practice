# MkDocs 与 GitHub Pages 自动部署实验

《开源软件设计与开发》实验二第二部分。

- 网站：https://dgklpd.github.io/mkdocs-pages-practice/
- 必需页面：首页、关于、使用指南、API 参考。
- main 保存源文件，GitHub Actions 构建后将 site 发布到 gh-pages。
- 在 Settings → Pages 中选择 Deploy from a branch、gh-pages、/(root)。

```bash
python -m pip install -r requirements.txt
mkdocs build --strict
mkdocs serve
```

工作流在 main 文档、配置或工作流变化时运行，也支持手动触发。部署使用仓库自带的 GITHUB_TOKEN，仅声明 contents: write，无需在仓库保存个人 Token。
