# OpenRocket 🚀（中文）

OpenRocket 是一个免费、功能齐全的模型火箭模拟器，让你在实际建造与发射之前先进行设计与仿真。

![Build Status](https://github.com/openrocket/openrocket/actions/workflows/build.yml/badge.svg)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
![GitHub release](https://img.shields.io/github/release/openrocket/openrocket.svg)
[![Github Releases (by release)](https://img.shields.io/github/downloads/openrocket/openrocket/latest/total.svg)](https://GitHub.com/openrocket/openrocket/releases/)
[![Read the Docs](https://readthedocs.org/projects/openrocket/badge/?version=latest)](https://openrocket.readthedocs.io/en/latest/)

[![snap release](https://snapcraft.io/openrocket/badge.svg)](https://snapcraft.io/openrocket)
![Chocolatey release](https://img.shields.io/chocolatey/v/openrocket)
[![Crowdin](https://badges.crowdin.net/openrocket/localized.svg)](https://crowdin.com/project/openrocket)
[![Join our Discord server!](https://img.shields.io/discord/1073297014814691328?logo=discord)](https://discord.gg/qD2G5v2FAw)

--------

## 🛠️ 设计、可视化与分析

1. **设计**：使用丰富的内置组件来构建你的火箭：
   ![Three-stage rocket - 2D](.github/OpenRocket_home_2D.png)

2. **可视化**：以 3D 方式展示你的作品：
   ![Three-stage rocket - 3D](.github/OpenRocket_home_3D.png)

3. **绘图与分析**：对仿真结果进行绘图与分析，以便提升精度：
   ![Three-stage rocket - Simulation plot](.github/OpenRocket_sim.png)

## 🌟 功能

- **六自由度飞行仿真**
- **自动化设计优化**
- **实时仿真高度、速度与加速度显示**
- **支持分级与集群**
- **导出至其他仿真程序（RockSim、RASAero II）**
- **将组件导出为 OBJ 文件以用于 3D 打印**
- **跨平台（基于 Java）**

... 以及更多功能

📖 了解更多信息请访问[我们的网站](https://openrocket.info/)。

## 💾 安装包

你可以在[这里](https://openrocket.info/downloads.html)找到 OpenRocket 安装包。

发行说明可在各个[发布页面](https://github.com/openrocket/openrocket/releases)或[我们的网站](https://openrocket.info/release_notes.html)上查看。

## 📖 文档

我们的文档托管在 [ReadTheDocs](https://openrocket.readthedocs.io/en/latest/)。

## 🚀 快速开始

**请查看[我们的文档](https://openrocket.readthedocs.io/en/latest/setup/getting_started.html)，其中提供了详细的快速入门指南。**

熟悉 OpenRocket 的最简单方式是打开程序内置的示例设计：

![Get started with the example designs](.github/getting-started.png)

从基础开始：调整组件尺寸、绘制仿真图、替换发动机……探索你的修改带来的影响，最重要的是享受这个过程！😊

---

## 📐 与 OpenRocket 相关的项目与工具
*注：如果你有想加入此列表的 OpenRocket 相关项目，可以提交一个新 issue。*

### 核心项目
| 项目                                                                               | 类型             | 说明                                                    |
|------------------------------------------------------------------------------------|------------------|---------------------------------------------------------|
| [openrocket/openrocket](https://github.com/openrocket/openrocket)                  | 核心项目         | 主模拟器（Java）                                        |
| [openrocket/openrocket.github.io](https://github.com/openrocket/openrocket.github.io) | 网站源代码     | 网站内容（Jekyll）                                      |
| [openrocket/openrocket-database](https://github.com/openrocket/openrocket-database) | 数据增强       | 扩展零件库（最初来自 [dbcook/openrocket-database](https://github.com/dbcook/openrocket-database)） |

### 集成与脚本
| 项目                                                                                 | 类型                       | 说明                                                                          |
|--------------------------------------------------------------------------------------|----------------------------|-------------------------------------------------------------------------------|
| [openrocket/orhelper](https://github.com/openrocket/orhelper)                        | 集成（Python）             | OpenRocket 的 Python 脚本/模块（通过 JPype）（源自 [SilentSys/orhelper](https://github.com/SilentSys/orhelper)） |
| [RocketPy-Team/RocketSerializer](https://github.com/RocketPy-Team/RocketSerializer) | 集成（Python）             | 将 `.ork` 文件转换为 RocketPy 兼容格式                                         |
| [SpaceTeam/ortools](https://github.com/SpaceTeam/ortools)                            | 集成工具（Python）         | 诸如 6DOF 着陆散布可视化等脚本                                                 |
| [schrum2/OpenRocketQD](https://github.com/schrum2/OpenRocketQD)                      | 优化工具（Python）         | 火箭设计的质量多样性优化                                                       |
| [waterloo-rocketry/or-monte-carlo](https://github.com/waterloo-rocketry/or-monte-carlo) | 仿真工具（Java）        | OpenRocket 的蒙特卡洛仿真封装                                                 |

### 发动机与空气动力扩展
| 项目                                                              | 类型                     | 说明                                   |
|-------------------------------------------------------------------|--------------------------|----------------------------------------|
| [SpaceTeam/ORLEG](https://github.com/SpaceTeam/ORLEG)             | 发动机建模（Python）     | OpenRocket 的液体发动机生成器         |
| [WPI-HPRC/ORBrake](https://github.com/WPI-HPRC/ORBrake) *(归档)*  | 插件（Java）             | 主动阻力控制（空气制动）               |

### 风与大气数据
| 项目                                    | 类型                     | 说明                                                                           |
|-----------------------------------------|--------------------------|--------------------------------------------------------------------------------|
| [ORWind](https://gpsdriftcast.com/orwind/) | 大气数据工具           | 获取/导入多层风场数据至 OpenRocket                                            |
| [Aloft](https://aloft.onrender.com/)      | 天气数据工具           | 获取飞行仿真的气象/大气剖面（风、温度、气压）                                  |

### 设计与 CAD 集成
| 项目                                                               | 类型          | 说明                                                                |
|--------------------------------------------------------------------|---------------|---------------------------------------------------------------------|
| [FreeCAD Rocket Workbench](https://github.com/davesrocketshop/Rocket) | CAD 工作台 | FreeCAD 的火箭设计工作台，可导入 OpenRocket `.ork` 文件             |

### 示例设计 / 展示
| 项目                                                                           | 类型        | 说明              |
|--------------------------------------------------------------------------------|-------------|-------------------|
| [TrinetraOne-OpenRocket](https://github.com/ChinmayBhattt/TrinetraOne-OpenRocket) | 示例设计 | 展示火箭项目      |

---

## 💪 参与贡献

让我们飞得更高！无论是实现新功能、编写文档，还是创建设计示例，每一份贡献都很重要。感兴趣？请查看[参与方式](https://openrocket.info/contribute.html)以及[贡献须知](CONTRIBUTING.md)。

### ✨ 贡献者
- [Sampo Niskanen](https://github.com/plaa) - 原始开发者
- [Doug Pedrick](https://github.com/rodinia814) - RockSim 设计、打印
- [Kevin Ruland](https://github.com/kruland2607) - Android 版本
- [Bill Kuker](https://github.com/bkuker) - 3D 可视化
- [Richard Graham](https://github.com/rdgraham) - 大地测量计算
- Jason Blood - 自由形状翼片集导入
- [Boris du Reau](https://github.com/bdureau) - 国际化
- [Daniel Williams](https://github.com/teyrana) - 吊舱支持、维护者
- [Joe Pfeiffer](https://github.com/JoePfeiffer) - 维护者
- [Billy Olsen](https://github.com/wolsen) - 维护者
- [Sibo Van Gool](https://github.com/SiboVG) - RASAero 文件格式、3D OBJ 导出、深色主题、维护者
- [Neil Weinstock](https://github.com/neilweinstock) - 测试、图标、论坛支持
- [H. Craig Miller](https://github.com/hcraigmiller) - 测试

你可以在[此处](https://github.com/openrocket/openrocket/graphs/contributors)查看完整贡献者列表。

### 🌍 译者
- Tripoli France
- Tripoli Spain
- Stefan Lobas / ERIG
- Mauro Biasutti
- Sky Dart Team / Ruslan V. Uss
- Vladimir Beran
- Polish Rocketry Society / Łukasz & Alex Kazanski
- Sibo Van Gool
- Mohamed Amin Elkebsi
- Oleksandr Hladin

## 📜 许可证

OpenRocket 以 [GNU GPL](https://www.gnu.org/licenses/gpl-3.0.en.html) 许可证开源发布。欢迎自由使用、学习与扩展。

---

⭐ 如果你觉得 OpenRocket 有帮助，请给我们点个星并分享给更多人！⭐

[![Star History Chart](https://api.star-history.com/svg?repos=openrocket/openrocket&type=Date)](https://star-history.com/#openrocket/openrocket&Date)

---

# OpenRocket 🚀

OpenRocket is a free, fully featured model rocket simulator that allows you to design and simulate your rockets before actually building and flying them.

![Build Status](https://github.com/openrocket/openrocket/actions/workflows/build.yml/badge.svg)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
![GitHub release](https://img.shields.io/github/release/openrocket/openrocket.svg)
[![Github Releases (by release)](https://img.shields.io/github/downloads/openrocket/openrocket/latest/total.svg)](https://GitHub.com/openrocket/openrocket/releases/)
[![Read the Docs](https://readthedocs.org/projects/openrocket/badge/?version=latest)](https://openrocket.readthedocs.io/en/latest/)

[![snap release](https://snapcraft.io/openrocket/badge.svg)](https://snapcraft.io/openrocket)
![Chocolatey release](https://img.shields.io/chocolatey/v/openrocket)
[![Crowdin](https://badges.crowdin.net/openrocket/localized.svg)](https://crowdin.com/project/openrocket)
[![Join our Discord server!](https://img.shields.io/discord/1073297014814691328?logo=discord)](https://discord.gg/qD2G5v2FAw)

--------

## 🛠️ Design, Visualize, and Analyze

1. **Design** your rockets using a rich selection of built-in components:
   ![Three-stage rocket - 2D](.github/OpenRocket_home_2D.png)

2. **Visualize** your masterpiece in 3D:
   ![Three-stage rocket - 3D](.github/OpenRocket_home_3D.png)

3. **Plot & Analyze** your simulation results for precision and improvements:
   ![Three-stage rocket - Simulation plot](.github/OpenRocket_sim.png)

## 🌟 Features

- **Six-degree-of-freedom flight simulation**
- **Automatic design optimization**
- **Realtime simulated altitude, velocity, and acceleration display**
- **Staging and clustering support**
- **Export to other simulation programs (RockSim, RASAero II)**
- **Export component(s) to OBJ file for 3D printing**
- **Cross-platform (Java-based)**

... plus many more

📖 Read more on [our website](https://openrocket.info/).

## 💾 Installers

You can find the OpenRocket installers [here](https://openrocket.info/downloads.html).

Release notes are available on each [release's page](https://github.com/openrocket/openrocket/releases) or on [our website](https://openrocket.info/release_notes.html).

## 📖 Documentation

You can find our documentation on [ReadTheDocs](https://openrocket.readthedocs.io/en/latest/).

## 🚀 Getting started

**Check out [our documentation](https://openrocket.readthedocs.io/en/latest/setup/getting_started.html) for a detailled guide on how to get started.**

The easiest way to get familiar with OpenRocket is to open one of our in-program example designs:

![Get started with the example designs](.github/getting-started.png)

Dive into the essentials: adjust component dimensions, plot a simulation, swap out motors, ... Explore the impact of your changes and, most importantly, enjoy the process! 😊

---

## 📐 OpenRocket-related Projects & Tools
*Note: If you have an OpenRocket-related project you would like included in the list, you can file a new issue for it.*

### Core Projects
| Project                                                                               | Type             | Description                                                    |
|---------------------------------------------------------------------------------------|------------------|----------------------------------------------------------------|
| [openrocket/openrocket](https://github.com/openrocket/openrocket)                     | Core project     | Main simulator (Java)                                          |
| [openrocket/openrocket.github.io](https://github.com/openrocket/openrocket.github.io) | Website source   | Website content (Jekyll)                                       |
| [openrocket/openrocket-database](https://github.com/openrocket/openrocket-database)   | Data enhancement | Expanded parts catalog (originally [dbcook/openrocket-database](https://github.com/dbcook/openrocket-database)) |

### Integration & Scripting
| Project                                                                                 | Type                       | Description                                                                         |
|-----------------------------------------------------------------------------------------|----------------------------|-------------------------------------------------------------------------------------|
| [openrocket/orhelper](https://github.com/openrocket/orhelper)                           | Integration (Python)       | Python scripting/module for OpenRocket (via JPype) (forked from [SilentSys/orhelper](https://github.com/SilentSys/orhelper)) |
| [RocketPy-Team/RocketSerializer](https://github.com/RocketPy-Team/RocketSerializer)     | Integration (Python)       | Convert `.ork` files to RocketPy-compatible formats                                 |
| [SpaceTeam/ortools](https://github.com/SpaceTeam/ortools)                               | Integration Tools (Python) | Scripts like 6DOF landing scatter visualization                                     |
| [schrum2/OpenRocketQD](https://github.com/schrum2/OpenRocketQD)                         | Optimization tool (Python) | Quality Diversity optimization for rocket designs                                   |
| [waterloo-rocketry/or-monte-carlo](https://github.com/waterloo-rocketry/or-monte-carlo) | Simulation tool (Java)     | Monte Carlo simulation wrapper for OpenRocket                                       |

### Engine & Aerodynamics Extensions
| Project                                                              | Type                     | Description                            |
|----------------------------------------------------------------------|--------------------------|----------------------------------------|
| [SpaceTeam/ORLEG](https://github.com/SpaceTeam/ORLEG)                | Engine modeling (Python) | Liquid-engine generator for OpenRocket |
| [WPI-HPRC/ORBrake](https://github.com/WPI-HPRC/ORBrake) *(archived)* | Plugin (Java)            | Active drag control (air-brakes)       |

### Wind & Atmospheric Data
| Project                                    | Type                     | Description                                                                          |
|--------------------------------------------|--------------------------|--------------------------------------------------------------------------------------|
| [ORWind](https://gpsdriftcast.com/orwind/) | Atmospheric data utility | Fetches/imports multi-level wind data for OpenRocket                                 |
| [Aloft](https://aloft.onrender.com/)       | Weather data utility     | Retrieves weather/atmospheric profiles (winds, temp, pressure) for flight simulation |

### Design & CAD Integration
| Project                                                               | Type          | Description                                                                   |
|-----------------------------------------------------------------------|---------------|-------------------------------------------------------------------------------|
| [FreeCAD Rocket Workbench](https://github.com/davesrocketshop/Rocket) | CAD workbench | A rocket design workbench for FreeCAD that can import OpenRocket `.ork` files |

### Example Designs / Showcase
| Project                                                                           | Type            | Description             |
|-----------------------------------------------------------------------------------|-----------------|-------------------------|
| [TrinetraOne-OpenRocket](https://github.com/ChinmayBhattt/TrinetraOne-OpenRocket) | Example designs | Showcase rocket project |

---

## 💪 Contribute

Help us soar higher! Whether it's implementing features, writing documentation, or creating design examples, every contribution matters. Interested? Check out [how to get involved](https://openrocket.info/contribute.html) and the [practicalities of contributing](CONTRIBUTING.md).

### ✨ Contributors
- [Sampo Niskanen](https://github.com/plaa) - Original developer
- [Doug Pedrick](https://github.com/rodinia814) - RockSim designs, printing
- [Kevin Ruland](https://github.com/kruland2607) - Android version
- [Bill Kuker](https://github.com/bkuker) - 3D visualization
- [Richard Graham](https://github.com/rdgraham) - Geodetic computations
- Jason Blood - Freeform fin set import
- [Boris du Reau](https://github.com/bdureau) - Internationalization
- [Daniel Williams](https://github.com/teyrana) - Pod support, maintainer
- [Joe Pfeiffer](https://github.com/JoePfeiffer) - Maintainer
- [Billy Olsen](https://github.com/wolsen) - Maintainer
- [Sibo Van Gool](https://github.com/SiboVG) - RASAero file format, 3D OBJ export, dark theme, maintainer
- [Neil Weinstock](https://github.com/neilweinstock) - Tester, icons, forum support
- [H. Craig Miller](https://github.com/hcraigmiller) - Tester

You can view the full list of contributors [here](https://github.com/openrocket/openrocket/graphs/contributors).

### 🌍Translators
- Tripoli France
- Tripoli Spain
- Stefan Lobas / ERIG
- Mauro Biasutti
- Sky Dart Team / Ruslan V. Uss
- Vladimir Beran
- Polish Rocketry Society / Łukasz & Alex Kazanski
- Sibo Van Gool
- Mohamed Amin Elkebsi
- Oleksandr Hladin

## 📜 License

OpenRocket is proudly open-source under the [GNU GPL](https://www.gnu.org/licenses/gpl-3.0.en.html) license. Feel free to use, study, and extend.

---
 
⭐ Please give us a star if you find OpenRocket useful, and spread the word! ⭐

[![Star History Chart](https://api.star-history.com/svg?repos=openrocket/openrocket&type=Date)](https://star-history.com/#openrocket/openrocket&Date)
