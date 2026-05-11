# vr-echizen-takefu

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A WebVR virtual tour of Echizen-Takefu Station, built with A-Frame. Explore a 3D model of the station in two different interactive modes.

This project is by [Code for FUKUI](https://github.com/code4fukui).

## Demos

-   [Ferris Wheel Mode (大観覧車モード)](https://code4fukui.github.io/vr-echizen-takefu/)
-   [Free Movement Mode (フリー移動モード)](https://code4fukui.github.io/vr-echizen-takefu/free.html)

## Features

-   **Two Viewing Modes:**
    -   **Ferris Wheel Mode:** A guided tour with an automatically rotating and elevating camera, set against a 360° photographic skybox of the actual location.
    -   **Free Movement Mode:** Explore the 3D model at your own pace using keyboard flight controls or VR teleportation.
-   **Cross-Platform:** Runs in any web browser with WebXR support, on desktop or in a VR headset.
-   **VR Ready:** Includes support for Oculus Touch controllers for teleport navigation.
-   **Lightweight:** Uses a single glTF (`.glb`) model with baked textures for efficient loading.

## Controls

### Ferris Wheel Mode (`index.html`)

-   **Mouse:** Click and drag to look around as the camera moves automatically.
-   **VR Headset:** Look around to change your viewpoint.

### Free Movement Mode (`free.html`)

-   **Keyboard & Mouse:**
    -   **Arrow Keys:** Move forward/backward and strafe left/right.
    -   **Mouse:** Look around.
    -   **Spacebar:** Ascend.
    -   **Shift:** Descend.
-   **VR Controllers (Oculus Touch):**
    -   **Trigger Button:** Aim and release to teleport.

## Technical Details

-   **3D Model:** `echizen-takefu_base.glb` (glTF format)
-   **360° Photo:** `vr-echizen-takefu.jpg` (Used as a skybox in Ferris Wheel Mode)
-   **Framework/Libraries:**
    -   [A-Frame](https://aframe.io) (v1.2.0)
    -   [aframe-teleport-controls](https://github.com/fernandojsg/aframe-teleport-controls)
    -   [mc-controls.js](https://code4fukui.github.io/glb-viewer/mc-controls.js) for keyboard flight controls.

## License

This project is licensed under the MIT License.