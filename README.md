# 初二拔优：因式分解专题讲义

面向已学提公因式、公式法和十字相乘的学生，供课后独立练习和复习。全书分为“因式分解的方法拓展”和“因式分解的应用”两章，可按专题使用。

正文有 26 道例题、27 道练习（含 1 道星号练习）和 2 道选学挑战，题号连续。例题附随文讲解，练习与挑战的解析放在各章末尾。

练习标题只留题号，便于学生自己判断方法。本版不保留章末入手提示；第二章保留回顾问题，用于检查条件和安排错题重做。

方法拓展章包括分组、拆项、配方、换元、主元法、因式定理和待定系数法；应用章包括条件求值、简便计算、非负性、整数方程、整除与几何问题。

部分题目选自或改编自《因式分解三讲总笔记》第 79 讲例 2、例 5 和第 80 讲例 2，对应例题 5、例题 7 和例题 25。

## 文件

- [因式分解-讲义.pdf](因式分解-讲义.pdf)：阅读与打印版。
- [因式分解-内容稿.md](因式分解-内容稿.md)：可编辑内容稿。
- [factorization-handout](factorization-handout)：LaTeX 源码及 Loom 文档类。

仓库只保留合订版。旧版讲义、原始材料、修改脚本及编译临时文件不纳入版本管理。

## 编辑和编译

修改时同步 Markdown 内容稿与 LaTeX 源码。进入 `factorization-handout`，用 XeLaTeX 编译两次：

```powershell
xelatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
xelatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
```

核对 `main.pdf` 后，将它复制为根目录的 `因式分解-讲义.pdf`。

- `main.tex`：版式和文档入口。
- `loom.cls`：Loom 文档类及字体选择。
- `sections/01-chapter.tex`：方法拓展正文与例题解析。
- `sections/02-chapter.tex`：应用正文与例题解析。
- `sections/90-solutions.tex`：第一章练习解析。
- `sections/91-solutions.tex`：第二章练习与挑战解析。

将 `main.tex` 中的 `\studentnotesfalse` 改为 `\studentnotestrue`，可隐藏小结、注意事项和方法补充卡；题目、回顾问题和解析仍保留。
