# 初二拔优：因式分解专题讲义

面向已学提公因式、公式法和十字相乘的学生。最终讲义将「因式分解的方法拓展」与「因式分解的应用」两章合订，按专题分多次授课，不固定课时。

正文含 25 道例题、27 道练习，另有 3 道选学挑战。例题解析紧跟题面，练习与挑战解析分别放在各章末尾。第一章例题编号为 1—13，第二章接为 14—25；第一章练习编号为 1—15，第二章接为 16—27。

方法拓展章包含因式定理专题：长除法、余式定理与因式定理的证明、有理根筛选、不同根与重因式，以及参数问题。

从《因式分解三讲总笔记》第79讲例2、例5和第80讲例2、例5选入均值换元、多字母主元法、四个连续整数积加1、三边关系判断形状，分别编为例题5、例题7、例题24和练习27。双整体换元、三项平方的交叉项核对、添1构造乘积及整除依据融入已有方法说明。

## 文件

- [因式分解-讲义.pdf](因式分解-讲义.pdf)：最终合并版讲义，可直接阅读或打印。
- [因式分解-内容稿.md](因式分解-内容稿.md)：最终内容稿，便于阅读和编辑。
- [factorization-handout](factorization-handout)：最终合并版的可编辑 LaTeX 源码，包含 Loom 文档类。

仓库仅保留最终合并版。旧版分章讲义、原始材料、修改记录、生成脚本、打包文件及编译临时文件不纳入版本管理。

## 编辑和编译

使用安装了所需宏包的 TeX Live 或 MiKTeX，以 XeLaTeX 编译。进入 `factorization-handout` 后执行两次：

```powershell
xelatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
xelatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
```

编译产物为 `factorization-handout/main.pdf`。确认排版后，可将它复制为根目录的 `因式分解-讲义.pdf`。

源码文件：

- `main.tex`：版式和文档入口。
- `loom.cls`：Loom 文档类及字体选择。
- `sections/01-chapter.tex`：方法拓展正文与例题解析。
- `sections/02-chapter.tex`：应用正文与例题解析。
- `sections/90-solutions.tex`：第一章练习与挑战解析。
- `sections/91-solutions.tex`：第二章练习与挑战解析。

将 `main.tex` 中的 `\studentnotesfalse` 改为 `\studentnotestrue`，可以隐藏入手提示、方法小结及易错提醒；例题随文解析及章末解析仍保留。

修改时请同步 Markdown 内容稿与 LaTeX 源码，并重新编译更新 PDF。
