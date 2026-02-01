# Occt_Qt_Sample

[English](../README.md) | [中文](./README_CN.md) | [日本語](./README_JP.md) | [한국어](./README_KO.md) | [русский](./README_RU.md)

---

## 한국어 (Korean)

### 소개
**Occt_Qt_Sample**은 **OpenCASCADE Technology (OCCT)**와 **Qt5**의 통합을 보여주는 템플릿 프로젝트입니다. CAD/CAM/CAE 애플리케이션 개발을 위한 기본 코드베이스 역할을 합니다. 이 프로젝트는 깔끔한 구조, 기본적인 3D 시각화 및 CAD 파일 가져오기/내보내기 기능을 제공하여 자체 프로젝트를 시작하기 위한 이상적인 출발점이 됩니다.

### 주요 기능
*   **CAD 파일 가져오기**: `.step`, `.stp`, `.iges`, `.igs`, `.brep` 파일 로딩 지원.
*   **CAD 파일 내보내기**: `.step`, `.iges`, `.brep` 형식으로 내보내기 지원.
*   **3D 시각화**: OpenCASCADE의 V3d_View 및 AIS를 기반으로 한 대화형 3D 뷰어.
*   **어셈블리 구조**: 가져온 CAD 어셈블리의 계층 구조를 트리 뷰로 표시.
*   **CMake 빌드 시스템**: 구성이 쉬운 CMake 빌드 설정.
*   **깔끔한 아키텍처**: 핵심 CAD 로직(`core_api`)과 UI(`ui`)의 분리.

### 시스템 요구 사항
*   **Qt 5**: 버전 5.12 이상 권장.
*   **OpenCASCADE Technology**: 버전 7.6.0 이상 권장.
*   **CMake**: 버전 3.19 이상.
*   **컴파일러**: C++17 호환 컴파일러 (MSVC, GCC, Clang).

### 빌드 방법

1.  **리포지토리 복제**:
    ```bash
    git clone https://github.com/your-username/Occt_Qt_Sample.git
    cd Occt_Qt_Sample
    ```

2.  **CMake 구성**:
    OpenCASCADE 설치 경로를 지정해야 합니다.
    ```bash
    mkdir build
    cd build
    cmake .. -DOpenCASCADE_DIR="C:/OpenCASCADE-7.6.0-vc14-64/opencascade-7.6.0"
    ```
    *참고: `OpenCASCADE_DIR`은 `OpenCASCADEConfig.cmake`가 포함된 디렉터리를 가리켜야 합니다.*

3.  **빌드**:
    ```bash
    cmake --build . --config Release
    ```

4.  **실행**:
    실행 파일(및 Windows의 경우 필요한 DLL)은 빌드 폴더(예: `build/Release`)에 위치합니다.