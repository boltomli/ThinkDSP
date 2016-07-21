# ThinkDSP

Allen B. Downey 所著 _Think DSP: Digital Signal Processing in Python_ 的 LaTeX 源文件 _中译_ 及 Python 代码。

本书（以及其它 _Think X_ 系列中的书）假定：如果你懂编程，你就可以通过编程技巧学习其它知识。

我写这本书的初衷是常见的数字信号处理教程均采取反向路径。大多数书（以及使用这些书的课程）自底而上地展示材料，从诸如相量（phasor）这样的数学抽象开始讲。

采用基于编程的路径，我可以自顶而下地马上开始呈现最重要的概念。到第一节结束，你就可以把一段声音分解为其谐波，修改谐波，并生成新的声音。

## 目前 Binder 无法安装 Python 3 版的 matplotlib，见其 [issue 39](https://github.com/binder-project/binder/issues/39) [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/boltomli/ThinkDSP)

本书尚在写作中，欢迎提出意见。

本书采用 Creative Commons 授权：

[Attribution-NonCommercial-ShareAlike 3.0 Unported](http://creativecommons.org/licenses/by-nc-sa/3.0/)

代码采用 GNU GPL：

[GNU GPLv3](http://www.gnu.org/licenses/gpl.html)

## 代码依赖

``` shell
for i in `cat requirements.txt`; do pip install --upgrade $i; done
jupyter nbextension enable --py --sys-prefix widgetsnbextension
```

在 ArchLinux 中亦可用：

``` shell
pacman -S --needed python-numpy python-scipy python-matplotlib python-pandas \
                   python-pillow python-scikit-image jupyter mathjax
```

在 Windows 中安装 scipy 和 scikit-image 较复杂，建议使用类似 [Anaconda](https://www.continuum.io) 这样的管理工具。

## 书的依赖

在 ArchLinux 中可用：

``` shell
pacman -S --needed texlive-most texlive-lang hevea evince
```

## Freesound

Special thanks to [Freesound](http://freesound.org), which is the source of many of the
sound samples I use in this book, and to the Freesound users who
uploaded those sounds.  I include some of their wave files in
the GitHub repository for this book, using the original file
names, so it should be easy to find their sources.

Unfortunately, most Freesound users don't make their real names
available, so I can only thank them using their user names.  Samples
used in this book were contributed by Freesound users: iluppai,
wcfl10, thirsk, docquesting, kleeb, landup, zippi1, themusicalnomad,
bcjordan, rockwehrmann, marchascon7, jcveliz.  Thank you all!

Here are links to the sources:

http://www.freesound.org/people/iluppai/sounds/100475/

http://www.freesound.org/people/wcfl10/sounds/105977/

http://www.freesound.org/people/Thirsk/sounds/120994/

http://www.freesound.org/people/ciccarelli/sounds/132736/

http://www.freesound.org/people/Kleeb/sounds/180960/

http://www.freesound.org/people/zippi1/sounds/18871/

http://www.freesound.org/people/themusicalnomad/sounds/253887/

http://www.freesound.org/people/bcjordan/sounds/28042/

http://www.freesound.org/people/rockwehrmann/sounds/72475/

http://www.freesound.org/people/marcgascon7/sounds/87778/

http://www.freesound.org/people/jcveliz/sounds/92002/
