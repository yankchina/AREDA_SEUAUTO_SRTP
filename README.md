# AREDA_SEUAUTO_SRTP

东南大学自动化学院 SRTP 项目 - AREDA (增强现实电路分析) 的公开代码库

## 项目简介

AREDA 是一个基于增强现实技术的电路分析教学工具，旨在通过AR技术提升电子电路学习的互动性和直观性。该项目结合了移动端AR应用和服务器端仿真计算，为用户提供沉浸式的电路学习体验。

## 项目结构

```
├── ios/                    # iOS 移动端应用
│   └── Ar trial/          # AR 试验应用
│       ├── ARapp/         # 主要AR应用模块
│       ├── ARChart/       # 图表显示组件
│       ├── ARScan/        # AR扫描相关功能
│       └── *.rcproject/   # Reality Composer项目文件
├── server/                # 服务器端代码
│   └── v1/               # 第一版服务器实现
├── docs/                 # 项目文档
│   ├── 2023/            # 2023年文档记录 (包含演示视频)
│   └── 2025/            # 2025年文档记录
└── README.md            # 项目说明文件
```



## 技术栈

### iOS 端
- **开发语言**: Swift
- **AR框架**: RealityKit, ARKit
- **UI框架**: SwiftUI
- **数据存储**: Core Data
- **开发工具**: Xcode, Reality Composer

### 服务器端
- **后端框架**: FastAPI (Python)
- **仿真计算**: MATLAB 引擎
- **API版本**: v1

## 主要功能

### iOS AR 应用
1. **电路识别与扫描** - 使用AR技术识别和扫描电路板
2. **交互式电路分析** - 实时显示电路参数和分析结果
3. **多种电路类型支持**:
   - 比例电路 (Proportional Circuit)
   - RC电路
   - RLC电路
   - 二阶滤波器 (Second Order Filter)
   - 序列发生器 (Sequence Generator)
   - 方波电路 (Square Wave)
   - 555定时器电路
4. **图表可视化** - 多线图表显示电路响应
5. **用户管理** - 登录、注册和用户数据管理

### 服务器功能
- **电路仿真计算** - 调用MATLAB进行精确的电路分析
- **API接口** - 为移动端提供数据和计算服务
- **用户数据管理** - 处理用户信息和学习记录

## 开发环境要求

### iOS 开发
- macOS 系统
- Xcode 12.0+
- iOS 14.0+
- 支持ARKit的iOS设备

### 服务器开发
- Python 3.8+
- MATLAB 引擎
- FastAPI 框架

## 项目演示

### 演示视频

我们提供了项目的演示视频，展示了AREDA AR电路分析应用的主要功能和使用方法：

📹 **何海心本科毕业设计项目演示视频**: [PresentationVideo.mp4](docs/2023/2023-06/2023-06-06/PresentationVideo.mp4) （2023-06-06）

> 该视频展示了如何使用AR技术进行电路识别、分析和可视化，以及各种电路类型的交互式学习体验。

## 快速开始

### 运行iOS应用
1. 使用Xcode打开 `ios/Ar trial/Ar trial.xcodeproj`
2. 连接支持ARKit的iOS设备
3. 编译并运行应用

### 启动服务器
```bash
cd server/v1
# 安装依赖和启动说明详见 server/v1/README.md
```

## 贡献者

- **何海心** - 本科毕业设计，提供了iOS端和服务器端的核心代码

## 项目状态

- ✅ iOS AR应用 - 基本功能完成
- 🚧 服务器端 - 开发中
- 📝 文档 - 持续更新中

## 许可证

详见 [LICENSE](LICENSE) 文件。

## 联系方式

如有问题或建议，请通过以下方式联系：
- 项目仓库: [AREDA_SEUAUTO_SRTP](https://github.com/yankchina/AREDA_SEUAUTO_SRTP)
- 所属机构: 东南大学自动化学院

---

*本项目为东南大学自动化学院 SRTP (Student Research Training Program) 项目的一部分。*
