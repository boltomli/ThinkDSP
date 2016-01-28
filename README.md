ThinkDSP
========

Allen B. Downey 所著 _Think DSP: Digital Signal Processing in Python_ 的 LaTeX 源文件 _中译_ 及 Python 代码。

本书（以及其它 _Think X_ 系列中的书）假定：如果你懂编程，你就可以通过编程技巧学习其它知识。

我写这本书的初衷是常见的数字信号处理教程均采取反向路径。大多数书（以及使用这些书的课程）自底而上地展示材料，从诸如相量（phasor）这样的数学抽象开始讲。

采用基于编程的路径，我可以自顶而下地马上开始呈现最重要的概念。到第一节结束，你就可以把一段声音分解为其谐波，修改谐波，并生成新的声音。

### 目前 Binder 无法安装 Python 3 版的 matplotlib，见其 [issue 39](https://github.com/binder-project/binder/issues/39) [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/boltomli/ThinkDSP)

本书尚在写作中，欢迎提出意见。

本书采用 Creative Commons 授权：

[Attribution-NonCommercial-ShareAlike 3.0 Unported](http://creativecommons.org/licenses/by-nc-sa/3.0/)

代码采用 GNU GPL：

[GNU GPLv3](http://www.gnu.org/licenses/gpl.html)

### 代码依赖

```
mkvirtualenv thinkdsp
for i in `cat requirements.txt`; do pip install --upgrade $i; done
```

在 ArchLinux 中亦可用：

```
pacman -S --needed python-numpy python-scipy python-matplotlib python-pandas \
                   python-pillow python-scikit-image jupyter mathjax
```

在 Windows 中安装 scipy 和 scikit-image 较复杂。以 Python 3.5 为例，安装好其它包后，从 [Unofficial Windows Binaries for Python Extension Packages](http://www.lfd.uci.edu/~gohlke/pythonlibs) 下载并单独安装如下：

```
pip install numpy matplotlib pandas pillow jupyter
pip install scipy-0.16.1-cp35-none-win_amd64.whl
pip install networkx-1.9.1-py2.py3-none-any.whl
pip install scikit_image-0.11.3-cp35-none-win_amd64.whl
```

### 书的依赖

在 ArchLinux 中可用：

```
pacman -S --needed texlive-most texlive-lang hevea evince
```
