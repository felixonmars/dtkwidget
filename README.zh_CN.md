## Deepin Tool Kit Widget

Deepint Tool Kit Core(DtkWidget) 提供各种UOS风格dtk基础控件.

您应该首先阅读 [Deepin应用程序规范](\ref doc/Specification).

## 依赖

### 编译依赖

* Qt >= 5.6

## 安装

### 从源代码构建

1. 确保已经安装了所有的编译依赖.
```bash
$ sudo apt build-dep ./
```
如果需要使用 `qtcreator` 的设计功能，可以 ：
```bash
$ sudo apt install qttools5-dev

# build
$ cmake ./plugin/dtkuiplugin -B build -DINSTALL_PLUGIN=ON -DCMAKE_INSTALL_PREFIX=/usr
$ cmake --build build -j$(nproc)

# install
$ cd build
$ sudo make install
```
2. 构建 `dtkwidget` :

```bash
$ cmake -B build
$ cmake --build build -j$(nproc)
```

3. 安装:

```bash
$ cd build
$ sudo make install
```

## 帮助

任何使用问题都可以通过以下方式寻求帮助:

* [Gitter](https://gitter.im/orgs/linuxdeepin/rooms)
* [IRC channel](https://webchat.freenode.net/?channels=deepin)
* [Forum](https://bbs.deepin.org)
* [WiKi](https://wiki.deepin.org/)

## 参与贡献

我们鼓励您报告问题并作出更改

* [开发者代码贡献指南](https://github.com/linuxdeepin/developer-center/wiki/Contribution-Guidelines-for-Developers)

## 协议

DTK工具包遵循协议 [LGPL-3.0-or-later](LICENSE).
