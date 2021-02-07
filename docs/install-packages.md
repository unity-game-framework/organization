# Install Packages

This guide explains how to install any package from the **Unity Game Framework** registry.

## Scoped Registry

In order to access to packages from different registries, rather than the default registry,
_Unity_ provides the way to define and use scoped registries with custom packages.

Read more about scoped registries:

> https://docs.unity3d.com/Manual/upm-scoped.html

## Manifest

Setup registry information directly in `manifest.json` file of the _Unity_ project.

This file located at _Unity_ project folder at specific path:

```
<Root of Unity project>\Packages\manifest.json
```

Open and edit file to add information for required registry.

Example of `manifest.json` file with zero dependencies and _Unity Game Framework_ registry:

```json
{
  "dependencies": {},
  "scopedRegistries": [
    {
      "name": "Unity Game Framework",
      "url": "https://unitygameframework.jfrog.io/artifactory/api/npm/default",
      "scopes": [
        "com.ugf"
      ]
    }
  ]
}
```
