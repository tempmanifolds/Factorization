# 因式分解专题讲义

供初二拔优学生课后独立练习和复习。例题附随文讲解，练习与挑战的解析集中在各章末尾。练习前不标明方法，必要的入手提示放在各章解析之前。

- `main.tex`：版式与文档入口。
- `sections/01-chapter.tex`：因式分解的方法拓展，含章末回顾与提示。
- `sections/02-chapter.tex`：因式分解的应用，含章末回顾与提示。
- `sections/90-solutions.tex`：第一章练习与挑战解析。
- `sections/91-solutions.tex`：第二章练习与挑战解析。
- `loom.cls`：Loom 文档类。

使用 XeLaTeX 编译两次：

```powershell
xelatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
xelatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
```

将 `main.tex` 的 `\studentnotesfalse` 改为 `\studentnotestrue`，可隐藏章末提示、小结和注意事项。回顾问题及解析仍保留。

修改后同步根目录的 `因式分解-内容稿.md`，核对排版，再将 `main.pdf` 复制为根目录的 `因式分解-讲义.pdf`。
