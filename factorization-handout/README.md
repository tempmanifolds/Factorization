# 因式分解专题讲义（两章合订）

使用 XeLaTeX 编译 `main.tex` 两次。例题的思路和解答紧跟题面；练习与挑战解析在书末。

- `sections/01-chapter.tex`：因式分解的方法拓展。
- `sections/02-chapter.tex`：因式分解的应用。
- `sections/90-solutions.tex`：练习与挑战解析。
- `loom.cls`：编译所需的 Loom 文档类。

修改这些文件即可继续编辑。将 `main.tex` 的 `\studentnotesfalse` 改为 `\studentnotestrue`，可隐藏入手提示、方法小结与易错提醒。

```powershell
xelatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
xelatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
```

编译完成后，核对 `main.pdf`，并更新根目录的 `因式分解-讲义.pdf` 与 `因式分解-内容稿.md`。
