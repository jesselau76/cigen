# 词根词缀记忆工坊

用[`https://pdfresources.com/`](https://pdfresources.com/)搜索到了一个词根PDF,从而引发这个idea，从其中自动抽取词根词缀与例词，构建交互式记忆 Web App。

在线 Pages 地址:
[https://jesselau76.github.io/cigen/](https://jesselau76.github.io/cigen/)

## 功能

- 词根/词缀检索与浏览
- 词根详情页（例词 + 拆解 + 中文释义）
- 闪卡训练（显示答案 / 记住 / 再看）
- 选择题训练（本地记录正确率）
- 本地学习进度保存（`localStorage`）

## 目录

- `scripts/extract_pdf_data.py`: 从 PDF 生成结构化数据
- `data/roots_affixes.json`: 解析输出
- `index.html` + `styles.css` + `app.js`: 前端应用

## 使用方式

1. 重新生成数据（可选）:
   ```bash
   python3 scripts/extract_pdf_data.py
   ```
2. 启动静态服务:
   ```bash
   python3 -m http.server 8080
   ```
3. 打开浏览器访问:
   `http://localhost:8080`

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=jesselau76/cigen&type=Date&theme=dark" />
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=jesselau76/cigen&type=Date" />
  <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=jesselau76/cigen&type=Date" />
</picture>


