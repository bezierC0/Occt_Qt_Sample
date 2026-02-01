# Occt_Qt_Sample

[English](../README.md) | [中文](./README_CN.md) | [日本語](./README_JP.md) | [한국어](./README_KO.md) | [русский](./README_RU.md)

---

## 中文 (Chinese)

### 简介
**Occt_Qt_Sample** 是一个展示如何将 **OpenCASCADE Technology (OCCT)** 与 **Qt5** 集成的模板项目。它旨在作为开发 CAD/CAM/CAE 应用程序的基础代码库。本项目提供了清晰的结构、基本的 3D 可视化以及 CAD 文件的导入/导出功能，是您构建自己项目的理想起点。

### 功能
*   **CAD 文件导入**: 支持加载 `.step`, `.stp`, `.iges`, `.igs`, 和 `.brep` 文件。
*   **CAD 文件导出**: 支持导出为 `.step`, `.iges`, 和 `.brep` 格式。
*   **3D 可视化**: 基于 OpenCASCADE V3d_View 和 AIS 的交互式 3D 查看器。
*   **装配结构**: 在树状视图中显示导入的 CAD 装配层级结构。
*   **CMake 构建系统**: 易于配置的 CMake 构建设置。
*   **清晰的架构**: 核心 CAD 逻辑 (`core_api`) 与 用户界面 (`ui`) 分离。

### 环境要求
*   **Qt 5**: 推荐 5.12 或更高版本。
*   **OpenCASCADE Technology**: 推荐 7.6.0 或更高版本。
*   **CMake**: 3.19 或更高版本。
*   **编译器**: 兼容 C++17 的编译器 (MSVC, GCC, Clang)。

### 编译指南

1.  **克隆仓库**:
    ```bash
    git clone https://github.com/your-username/Occt_Qt_Sample.git
    cd Occt_Qt_Sample
    ```

2.  **通过 CMake 配置**:
    您需要指定 OpenCASCADE 的安装路径。
    ```bash
    mkdir build
    cd build
    cmake .. -DOpenCASCADE_DIR="C:/OpenCASCADE-7.6.0-vc14-64/opencascade-7.6.0"
    ```
    *注意: `OpenCASCADE_DIR` 应指向包含 `OpenCASCADEConfig.cmake` 的目录。*

3.  **构建**:
    ```bash
    cmake --build . --config Release
    ```

4.  **运行**:
    可执行文件（以及 Windows 上所需的 DLL）将位于构建文件夹中（例如 `build/Release`）。

---