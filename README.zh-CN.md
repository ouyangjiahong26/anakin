# Anakin

简体中文 | [English](README.md)

[![DOI](https://zenodo.org/badge/143483510.svg)](https://zenodo.org/badge/latestdoi/143483510)

Anakin（Aerospace eNgineer's Assistant for Kinematics, Inertia and dyNamics）是一个 Matlab 框架，定义了一组类，用于简化航空航天工程及其他学科中经典力学问题的建模与求解。

![Anakin logo](docs/anakin-logo.png)

## 安装

安装时只需[下载 Anakin](https://github.com/mariomerinomartinez/anakin/archive/master.zip)，并将根目录添加到 Matlab 路径。

### 依赖

运行代码需要较新版本的 Matlab（R2016a 或更高版本）。使用大部分功能需要 [Symbolic Math Toolbox](https://www.mathworks.com/products/symbolic.html)。建议使用 R2018a 或更高版本，因为它支持示例实时脚本。

目前正在将 Anakin 移植到 Octave。如果你愿意参与这项工作，请联系我们。

## 快速使用指南

Anakin 的文档位于 `/docs` 子目录。每个 Anakin 类都有一个实时脚本，介绍其用法和功能。`/problems` 子目录包含用于求解 Universidad Carlos III de Madrid 航空航天工程本科课程 'Mechanics Applied to Aerospace Engineering' 习题的实时脚本。

使用 Anakin 时，建议先导入整个 Anakin 包：

```Matlab
import anakin.*
```

如果不这样做，则需要通过 `anakin.` 前缀访问所有类，例如 `anakin.basis`。

目前 Anakin 定义了以下类：

* `tensor`：标量、向量、张量的通用类
* `basis`：向量基
* `frame`：参考坐标系
* `point`：几何点
* `particle`：质点
* `body`：刚体

每个类的属性和方法的说明见各代码文件的头部注释。更多信息和用法示例见 `/docs` 目录中的实时脚本。

### 测试

单元测试位于 `/tests` 子目录。将 Anakin 包添加到 Matlab 路径后，在该子目录中执行 `runtests` 即可运行全部测试。

## 参与贡献

如果你有改进意见，或有意参与本项目及其他代码的持续开发，请[联系我们](mailto:mario.merino@uc3m.es)。

## 致谢

本程序源于 Universidad Carlos III de Madrid 航空航天工程系的大量工作。本项目以开源形式发布，希望它能对他人有所帮助。如果你觉得它有用，或在任何工作中使用了它，我们希望你通过引用以下文献来致谢：

Mario Merino (2018). [https://github.com/uc3m-aerospace/anakin](https://github.com/uc3m-aerospace/anakin): First release [DOI:10.5281/zenodo.2533336](https://doi.org/10.5281/zenodo.2533336)

## 许可证

Copyright (c) 2018 Mario Merino. 本软件以 MIT 许可证开源发布，详见 [LICENSE.md](LICENSE.md)。
