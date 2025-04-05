
## 📦 Visual AI with Gemini: Detection, Captioning, Reasoning, OCR

Object detection is a core task in computer vision, enabling systems to identify and localize objects, features, or areas of interest within images. With the advent of multimodal large language models like Google’s **Gemini 2.0 Flash** and **Gemini 2.5 Pro**, these capabilities can now be harnessed using **natural language prompts**—removing the need for traditional fine-tuning workflows or large annotated datasets.

This project demonstrates how to leverage Gemini for advanced visual understanding across three main areas:

### 🔍 1. Detection
Gemini can detect and return **2D bounding boxes** around relevant regions in an image—such as objects, anomalies, or landmarks—based entirely on user-defined natural language prompts. No prior training or fine-tuning is required.

✅ **Prompt Used**: `"Detect the 2d bounding boxes"`

📦 **Output Format**: Coordinates are returned as `[y1, x1, y2, x2]` and **normalized to a [0, 1000] scale**. When visualizing, make sure to **denormalize** these values relative to the actual image size.


<img src="https://github.com/janithaDassanayake/dummyimages/blob/main/download%20(13).png" alt="Gemini 2.5 Pro Experimental Benchmarks1" />

<br>
### 🧠 2. Visual Reasoning
Beyond simple detection, Gemini supports **visual reasoning**—enabling it to:
- Understand spatial relationships
- Differentiate between visually similar objects
- Infer context and complexity of scenes
- Draw human-like conclusions from visual data

This allows for more nuanced and intelligent interaction with images using just natural language.

<img src="https://github.com/janithaDassanayake/dummyimages/blob/main/download%20(14).png" alt="Gemini 2.5 Pro Experimental Benchmarks" />

<br>
### 🖋️ 3. Visual Captioning
Gemini can generate detailed, human-like **captions** that describe:
- Shapes, colors, textures
- Object structure and layout
- Scene context and interactions

These captions enhance explainability and are useful for applications like content summarization, accessibility, automation, and visual documentation.


<img src="https://github.com/janithaDassanayake/dummyimages/blob/main/ddddddd.JPG" alt="Gemini 2.5 Pro Experimental Benchmarks3" />

### 🛠️ Technical Notes

- 💡 **Models**: Uses either `Gemini 2.0 Flash` (fast) or `Gemini 2.5 Pro` (more accurate).
- 📜 **Bounding Box Schema**: Defined using Pydantic (Python) for clean and robust data handling.
- 🔤 **Additional Tasks Supported**: Optical Character Recognition (OCR), image-text reasoning, and scene interpretation.
