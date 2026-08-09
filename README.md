# 抽象代数讲义

本仓库保存抽象代数讲义的手写原稿与 LaTeX 电子版。电子版按照数学内容组织章节，不按授课周次划分。

## 当前内容

- 第一章：群
  - 群的定义与基本性质
  - 子群
  - 生成子群与循环群
  - 对称群与置换群
  - 陪集

手写原稿见 [`week1.pdf`](week1.pdf)，编译后的电子讲义见 [`abstract-algebra-notes.pdf`](abstract-algebra-notes.pdf)。

## 编译

本项目使用 `ctexbook` 文档类。安装 TeX Live 后，在仓库根目录运行：

```bash
latexmk -xelatex -interaction=nonstopmode -halt-on-error \
  -jobname=abstract-algebra-notes main.tex
```

章节源文件位于 `chapters/`；后续内容可继续按主题新增章节，并在 `main.tex` 中引入。
