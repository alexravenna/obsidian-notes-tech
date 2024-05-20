---
documentation:
  - https://learn.microsoft.com/en-us/azure/remote-rendering/
aliases:
  - ARR
tags:
  - microsoft
  - azure
---
# Description
- Enables real-time streaming of high-quality, interactive 3D content to devices like the [[HoloLens 2]]
- Basically, high-end [[GPU]]s in the [[Azure]] cloud are used to render models at a higher fidelity than possible on a device such as the HoloLens
	- These renders are then streamed as video to the device
	- Elements can still be rendered locally on the device: Hybrid Rendering
	- For extremely complex models, the workload can be distributed to multiple GPUs
- Models have to be in a proprietary binary format - [[FBX]] and [[GLTF]] can't be used
# Azure Remote Rendering Toolkit
- Open-source desktop application
- Developed in [[C++]]/[[Qt]]
- Source: [Azure/azure-remote-rendering-asset-tool: Azure Remote Rendering Toolkit (ARRT) assists with uploading, converting, and rendering 3D models using the Azure Remote Rendering service. (github.com)](https://github.com/Azure/azure-remote-rendering-asset-tool)