# Occt_Qt_Sample

[English](../README.md) | [中文](./README_CN.md) | [日本語](./README_JP.md) | [한국어](./README_KO.md) | [русский](./README_RU.md)

---

## 日本語 (Japanese)

### はじめに
**Occt_Qt_Sample** は、**OpenCASCADE Technology (OCCT)** と **Qt5** を統合したテンプレートプロジェクトです。CAD/CAM/CAE アプリケーション開発の基礎コードベースとして機能します。このプロジェクトは、明確な構造、基本的な 3D ビジュアライゼーション、CAD ファイルのインポート/エクスポート機能を提供し、独自のプロジェクトを開始するための理想的な雛形となります。

### 機能
*   **CAD ファイルのインポート**: `.step`, `.stp`, `.iges`, `.igs`, `.brep` ファイルの読み込みをサポート。
*   **CAD ファイルのエクスポート**: `.step`, `.iges`, `.brep` 形式への書き出しをサポート。
*   **3D ビジュアライゼーション**: OpenCASCADE の V3d_View および AIS に基づくインタラクティブな 3D ビューア。
*   **アセンブリ構造**: インポートされた CAD アセンブリの階層構造をツリービューで表示。
*   **CMake ビルドシステム**: 設定が容易な CMake ビルド環境。
*   **クリーンなアーキテクチャ**: コア CAD ロジック (`core_api`) と UI (`ui`) の分離。

### 必要要件
*   **Qt 5**: バージョン 5.12 以上推奨。
*   **OpenCASCADE Technology**: バージョン 7.6.0 以上推奨。
*   **CMake**: バージョン 3.19 以上。
*   **コンパイラ**: C++17 互換コンパイラ (MSVC, GCC, Clang)。

### ビルド方法

1.  **リポジトリのクローン**:
    ```bash
    git clone https://github.com/your-username/Occt_Qt_Sample.git
    cd Occt_Qt_Sample
    ```

2.  **CMake での設定**:
    OpenCASCADE のインストールパスを指定する必要があります。
    ```bash
    mkdir build
    cd build
    cmake .. -DOpenCASCADE_DIR="C:/OpenCASCADE-7.6.0-vc14-64/opencascade-7.6.0"
    ```
    *注意: `OpenCASCADE_DIR` は `OpenCASCADEConfig.cmake` が含まれているディレクトリを指定してください。*

3.  **ビルド**:
    ```bash
    cmake --build . --config Release
    ```

4.  **実行**:
    実行ファイル（および Windows の場合は必要な DLL）は、ビルドフォルダ（例: `build/Release`）に作成されます。

---