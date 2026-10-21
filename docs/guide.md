# 使用指南

## 自动发布流程

1. 编写或修改 Markdown 文档。
2. 提交代码到 GitHub 的 main 分支。
3. GitHub Actions 自动安装依赖、构建并部署。
4. 在 Actions 查看运行结果，再打开 Pages 地址验证页面。

## 本地预览

```bash
python -m pip install -r requirements.txt
mkdocs serve
```

根据终端显示的地址访问本地预览。

## 构建检查

```bash
mkdocs build --strict
```

静态文件生成到 site 目录。自动部署工作流将其发布到 gh-pages 分支；在仓库 Pages 设置中选择该分支的根目录。
