# Install Packages

This guide explains how to install any package from the **Unity Game Framework** registry.

## List

Documentation has list of all packages in one place with package version and other information.

[Repositories List](repositories.md)

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

## Preview Packages

Some packages have _Preview_ version of package, with latest changes and features,
but some of this packages will not work with _Non-Preivew_ versions of dependencies.

If package have preview version and other dependencies, it is **recommened** to update all dependencies to preview versions.

To display preview versions of packages, changing _Package Manager_ settings required.

Read about _Package Manager Advaced Settings_:

> https://docs.unity3d.com/2021.1/Documentation/Manual/class-PackageManager.html
