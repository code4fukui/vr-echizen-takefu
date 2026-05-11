# vr-echizen-takefu

A-Frameを使用したWebVRによる越前武生駅のバーチャルツアーです。2つのインタラクティブモードで駅の3Dモデルを探索できます。

このプロジェクトは [Code for FUKUI](https://github.com/code4fukui) によって作成されました。

## デモ

-   [大観覧車モード](https://code4fukui.github.io/vr-echizen-takefu/)
-   [フリー移動モード](https://code4fukui.github.io/vr-echizen-takefu/free.html)

## 特徴

-   **2つの表示モード:**
    -   **大観覧車モード:** 実際の場所の360°写真のスカイボックスを背景に、カメラが自動的に回転・昇降するガイド付きツアー。
    -   **フリー移動モード:** キーボードによる飛行操作またはVRテレポート機能を使って、自分のペースで3Dモデルを自由に探索。
-   **クロスプラットフォーム:** WebXRをサポートする任意のウェブブラウザで動作します（デスクトップおよびVRヘッドセットに対応）。
-   **VR対応:** Oculus Touchコントローラーによるテレポートナビゲーションをサポート。
-   **軽量設計:** テクスチャを焼き込んだ単一のglTF（`.glb`）モデルを使用し、効率的な読み込みを実現。

## 操作方法

### 大観覧車モード (`index.html`)

-   **マウス:** カメラが自動的に移動する中、クリック＆ドラッグで周囲を見渡すことができます。
-   **VRヘッドセット:** 周囲を見渡して視点を変更します。

### フリー移動モード (`free.html`)

-   **キーボード & マウス:**
    -   **矢印キー:** 前後・左右に移動。
    -   **マウス:** 周囲を見渡す。
    -   **スペースバー:** 上昇。
    -   **Shiftキー:** 下降。
-   **VRコントローラー（Oculus Touch）:**
    -   **トリガーボタン:** 狙いを定めて離すとテレポートします。

## 技術的詳細

-   **3Dモデル:** `echizen-takefu_base.glb`（glTF形式）
-   **360°写真:** `vr-echizen-takefu.jpg`（大観覧車モードでスカイボックスとして使用）
-   **フレームワーク/ライブラリ:**
    -   [A-Frame](https://aframe.io)（v1.2.0）
    -   [aframe-teleport-controls](https://github.com/fernandojsg/aframe-teleport-controls)
    -   [mc-controls.js](https://code4fukui.github.io/glb-viewer/mc-controls.js)（キーボード飛行操作用）

## ライセンス

このプロジェクトは MIT License の下で公開されています。
