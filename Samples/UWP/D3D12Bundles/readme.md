---
page_type: sample
languages:
- cpp
products:
- windows
- windows-uwp
name: Direct3D 12 bundles sample
urlFragment: d3d12-bundles-sample-uwp
description: Demonstrates the use of Direct3D 12 bundles.
extendedZipContent:
- path: LICENSE
  target: LICENSE
---

# Direct3D 12 bundles sample

![Bundles GUI](src/D3D12Bundles.png)

This sample demonstrates the use of Direct3D 12 bundles. An app can use bundles to group a small number of API commands together for execution later. When a bundle is created, the driver will perform as much pre-processing as possible to make it inexpensive to execute the bundle later. Part of this pre-processing means that there are certain restrictions on what operations can be performed within a bundle.

## Optional features

This sample has been updated to build against the Windows 10 Anniversary Update SDK. In this SDK a new revision of Root Signatures is available for Direct3D 12 apps to use. Root Signature 1.1 allows for apps to declare when descriptors in a descriptor heap won't change or the data descriptors point to won't change.  This allows the option for drivers to make optimizations that might be possible knowing that something (like a descriptor or the memory it points to) is static for some period of time.
