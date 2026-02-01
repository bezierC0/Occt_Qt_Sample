# Occt_Qt_Sample

[English](README.md) | [中文](./doc/README_CN.md) | [日本語](./doc/README_JP.md) | [한국어](./doc/README_KO.md) | [русский](./doc/README_RU.md)

---

## English

### Introduction
**Occt_Qt_Sample** is a template project demonstrating the integration of **OpenCASCADE Technology (OCCT)** with **Qt5**. It serves as a foundational codebase for developing CAD/CAM/CAE applications. This project provides a clean structure, basic 3D visualization, and CAD file import/export capabilities, making it an ideal starting point for your own projects.

### Features
*   **CAD File Import**: Supports loading `.step`, `.stp`, `.iges`, `.igs`, and `.brep` files.
*   **CAD File Export**: Supports exporting to `.step`, `.iges`, and `.brep` formats.
*   **3D Visualization**: Interactive 3D viewer based on OpenCASCADE's V3d_View and AIS (Application Interactive Services).
*   **Assembly Structure**: Displays the hierarchy of the imported CAD assembly in a tree view.
*   **CMake Build System**: Easy-to-configure CMake build setup.
*   **Clean Architecture**: Separation of Core CAD logic (`core_api`) and UI (`ui`).

### Requirements
*   **Qt 5**: Version 5.12 or higher recommended.
*   **OpenCASCADE Technology**: Version 7.6.0 or higher recommended.
*   **CMake**: Version 3.19 or higher.
*   **Compiler**: C++17 compatible compiler (MSVC, GCC, Clang).

### Build Instructions

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/Occt_Qt_Sample.git
    cd Occt_Qt_Sample
    ```

2.  **Configure with CMake**:
    You need to specify the path to your OpenCASCADE installation.
    ```bash
    mkdir build
    cd build
    cmake .. -DOpenCASCADE_DIR="C:/OpenCASCADE-7.6.0-vc14-64/opencascade-7.6.0"
    ```
    *Note: `OpenCASCADE_DIR` should point to the directory containing `OpenCASCADEConfig.cmake`.*

3.  **Build**:
    ```bash
    cmake --build . --config Release
    ```

4.  **Run**:
    The executable (and necessary DLLs on Windows) will be in the build folder (e.g., `build/Release`).

---





