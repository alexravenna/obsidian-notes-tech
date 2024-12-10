---
created: 2024-06-06T15:55:05Z
updated: 2024-12-10T08:34:58Z
tags:
  - computer-vision
documentation:
  - https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/
training:
  - https://learn.microsoft.com/en-us/training/paths/create-computer-vision-solutions-azure-ai/
---
# Description
- Studio link: [Vision Studio (azure.com)](https://portal.vision.cognitive.azure.com/gallery/featured)
- An [[Azure AI Services|Azure AI Service]] that provides functionality for:
	- Captioning and generating tags for images
	- Object detection
	- People detection
	- Image metadata, color and type analysis
	- Category identification
	- Background removal
	- Moderation rating
	- [[OCR]]
	- Smart [[thumbnail]] generation - a region of interest can be determined and used
	  
# Development
- With the [[Csharp|C#]] [[SDK]]:
```csharp
using Azure.AI.Vision.ImageAnalysis;

ImageAnalysisClient client = new ImageAnalysisClient(
    Environment.GetEnvironmentVariable("ENDPOINT"),
    new AzureKeyCredential(Environment.GetEnvironmentVariable("KEY")));

ImageAnalysisResult result = client.Analyze(
    new Uri("<url>"),
    VisualFeatures.Caption | VisualFeatures.Read,
    new ImageAnalysisOptions { GenderNeutralCaption = true });
```
- `VisualFeatures` defines which functionalities (see above) should be utilized and returned in the result