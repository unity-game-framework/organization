# Install Packages

This guide explains how to install any package from the **Unity Game Framework** registry.

## Scoped registry

Setup **Unity Game Framework** scoped registry in project `manifest.json` file and packages become available through the **Unity Package Manager** window.

Read more about scoped registries: https://docs.unity3d.com/Manual/upm-scoped.html

## Example

Example how to setup registry of the **Unity Game Framework** in project using **Unity 2019.3**.

```json
{
  "scopedRegistries": [
    {
      "name": "Unity Game Framework",
      "url": "https://api.bintray.com/npm/unity-game-framework/public",
      "scopes": [
        "com.ugf"
      ]
    }
  ]
}
```
