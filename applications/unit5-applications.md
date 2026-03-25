# Unit 5 Applications: AI in Engineering & CAD/CAM

---

## Guided Exercise 1: Image-to-3D Lab

### Objective
Convert a 2D photograph into a 3D model using Meshy.ai and evaluate the output quality.

### Step-by-Step Instructions

1. **Prepare Your Image**
   - Select a simple object with clear geometry (a coffee mug, a bolt, a bracket).
   - Photograph it against a plain, contrasting background.
   - Use even lighting with no harsh shadows.
   - Capture from a 3/4 angle so the tool can infer depth.

2. **Upload to Meshy.ai**
   - Go to [meshy.ai](https://www.meshy.ai) and sign in (free tier is sufficient).
   - Select **Image to 3D**.
   - Upload your photograph.
   - Choose the **Medium** quality preset for a balance of speed and detail.
   - Click **Generate** and wait for processing (typically 1-3 minutes).

3. **Download and View the Model**
   - Once generated, download the model in **.GLB** format (most compatible).
   - Open the file in a 3D viewer:
     - **Windows**: 3D Viewer (built-in) or import into Fusion 360.
     - **Web**: Use [gltf-viewer.donmccurdy.com](https://gltf-viewer.donmccurdy.com).
   - Rotate the model to inspect all sides.

4. **Evaluate Quality**
   Complete this assessment for your model:

   | Quality Criterion          | Rating (1-5) | Notes                          |
   |----------------------------|:------------:|--------------------------------|
   | Overall shape accuracy     |              |                                |
   | Surface detail retention   |              |                                |
   | Symmetry (if applicable)   |              |                                |
   | Texture/color fidelity     |              |                                |
   | Mesh cleanliness           |              |                                |
   | Suitability for 3D printing|              |                                |

5. **What to Look For**
   - **Good signs**: Clean edges, proportional dimensions, recognizable shape from all angles.
   - **Common issues**: Holes in the mesh, distorted back surfaces, blobby geometry on thin features.
   - **Deal-breakers for manufacturing**: Non-watertight mesh, inverted normals, extreme polygon count.

### Troubleshooting
- **Model looks flat or pancake-shaped**: Your photo was taken too straight-on. Retake from a 30-45 degree angle.
- **Texture is blurry or misaligned**: Ensure the original image is at least 1024x1024 pixels.
- **Download fails or format is unrecognized**: Try exporting as .OBJ instead of .GLB. Some viewers handle OBJ better.

---

## Guided Exercise 2: Vectorization Test

### Objective
Convert a raster image to vector format using Vectorizer.ai and compare input versus output quality.

### Step-by-Step Instructions

1. **Select a Test Image**
   - Use a logo, technical drawing, or line-art diagram (PNG or JPG).
   - For best comparison, choose an image with both sharp edges and gradients.

2. **Upload to Vectorizer.ai**
   - Go to [vectorizer.ai](https://vectorizer.ai).
   - Drag and drop your image onto the upload area.
   - Wait for the automatic conversion to complete.

3. **Download and Compare**
   - Download the output as **SVG**.
   - Open both the original raster and the SVG side by side.
   - Zoom in to 400% on both images.

4. **Comparison Matrix**

   | Feature                | Original Raster | Vectorized SVG |
   |------------------------|:---------------:|:--------------:|
   | File size              |                 |                |
   | Clarity at 400% zoom   |                 |                |
   | Edge sharpness         |                 |                |
   | Color accuracy         |                 |                |
   | Gradient handling      |                 |                |
   | Scalability            |                 |                |
   | Editability in CAD     |                 |                |

5. **Key Questions to Answer**
   - At what zoom level does the raster image become pixelated while the vector remains sharp?
   - Were any fine details lost during conversion?
   - Could the vector output be directly imported into a CAD program for machining?

### Troubleshooting
- **Output looks overly simplified**: The source image may be too low-resolution. Use an image of at least 300 DPI.
- **Curves appear jagged in the SVG**: Open the SVG in a vector editor (Inkscape, Illustrator) and check node count. Over-simplification reduces curves to straight segments.
- **Colors don't match**: Some vectorizers reduce the color palette. Check settings for color fidelity options.

---

## Guided Exercise 3: Reverse Engineering Workflow

### Objective
Photograph a real object, generate a 3D model using AI, then compare the digital model's dimensions against the physical object.

### Step-by-Step Instructions

1. **Select and Measure the Physical Object**
   - Choose a simple object you can measure accurately (a block, a fitting, a handle).
   - Using calipers or a ruler, record at least 5 key dimensions:
     - Overall length, width, height
     - At least 2 feature dimensions (hole diameter, slot width, etc.)

2. **Photograph the Object**
   - Take 4-8 photos from different angles.
   - Include a reference object of known size (ruler, coin) in at least one photo.
   - Maintain consistent lighting across all shots.

3. **Generate the 3D Model**
   - Upload to **Luma AI** (for photogrammetry-style reconstruction) or **TripoSR** (for single-image inference).
   - For Luma AI: Upload multiple images for better reconstruction.
   - For TripoSR: Upload the best single 3/4-angle image.
   - Download the resulting model.

4. **Measure the Digital Model**
   - Import the model into Fusion 360, FreeCAD, or an online viewer with measurement tools.
   - Scale the model using your reference object dimension.
   - Measure the same 5 dimensions you recorded physically.

5. **Dimension Comparison Table**

   | Dimension         | Physical (mm) | Digital (mm) | Difference (mm) | Error (%) |
   |-------------------|:-------------:|:------------:|:----------------:|:---------:|
   | Overall Length    |               |              |                  |           |
   | Overall Width     |               |              |                  |           |
   | Overall Height    |               |              |                  |           |
   | Feature 1:        |               |              |                  |           |
   | Feature 2:        |               |              |                  |           |

6. **Analysis Questions**
   - Which dimensions had the highest error? Why?
   - Is the accuracy sufficient for: (a) visual reference, (b) 3D printing a replacement, (c) precision machining?
   - What would improve the accuracy?

### Troubleshooting
- **Model is not to scale**: AI-generated models have no inherent scale. You must manually scale using a known reference dimension.
- **Features are missing or merged**: Small holes, thin walls, and internal features are commonly lost. These must be added manually in CAD.
- **Model orientation is wrong**: Use the alignment tools in your CAD software to reorient the model to match standard views.

---

## Guided Exercise 4: Generative Design Concept

### Objective
Understand how generative design works by discussing a real design challenge and mapping out how Fusion 360's generative design would approach it.

### Discussion Framework

1. **Choose a Design Challenge**
   Pick one (or propose your own):
   - A mounting bracket that supports a 50 kg load
   - A structural support connecting two beams at a 90-degree angle
   - A cable routing connector that must fit within a 100mm x 60mm x 40mm envelope

2. **Define the Design Space**
   For your chosen challenge, specify:
   - **Preserve regions**: What geometry must remain fixed? (Mounting holes, connection surfaces)
   - **Obstacle regions**: Where can material NOT go? (Clearance zones, access paths)
   - **Design space**: The maximum volume available for the design.

3. **Define Constraints and Objectives**
   - **Load cases**: What forces act on the part? Direction, magnitude, type (static, cyclic).
   - **Material**: What material would you specify? (Aluminum 6061, Steel, Nylon)
   - **Manufacturing method**: How will it be made? (CNC milling, 3D printing, casting)
   - **Objective**: Minimize mass? Maximize stiffness? Minimize cost?

4. **Predict the Outcome**
   - Sketch what you think the generative design result would look like.
   - Generative design typically produces organic, bone-like structures. Why?
   - How would the result differ if you changed the manufacturing method from 3D printing to CNC milling?

5. **Compare to Traditional Design**
   - How would a human engineer traditionally design this part?
   - What advantages does generative design offer?
   - What are the limitations? (Aesthetics, manufacturability, trust)

### Troubleshooting
- **Unsure how to define load cases**: Start with the simplest case: a single static force in one direction. You can add complexity later.
- **Design space seems too abstract**: Think of it as a block of clay. Preserve regions are areas you cannot cut. Obstacle regions are areas already carved away. Everything else is where the algorithm decides.

---

## Independent Practice

### Practice 1: Complexity Scaling Test
1. Photograph **3 objects** of increasing complexity:
   - **Simple**: A box, cylinder, or block (minimal features).
   - **Medium**: A bracket, fitting, or handle (some curves and holes).
   - **Complex**: A gear, impeller, or organically shaped part.
2. Upload each to an image-to-3D tool (Meshy.ai or TripoSR).
3. Document your findings:

   | Object      | Complexity | Shape Accuracy | Detail Retention | Usable for Engineering? |
   |-------------|:----------:|:--------------:|:----------------:|:-----------------------:|
   | Object 1    | Simple     |                |                  |                         |
   | Object 2    | Medium     |                |                  |                         |
   | Object 3    | Complex    |                |                  |                         |

4. Write a short summary: At what complexity level do current AI tools stop being useful for engineering?

### Practice 2: Tool Comparison
1. Select one object from Practice 1.
2. Process it through both **Meshy.ai** and **TripoSR**.
3. Compare the two outputs:

   | Criterion            | Meshy.ai | TripoSR | Winner |
   |----------------------|:--------:|:-------:|:------:|
   | Processing speed     |          |         |        |
   | Geometric accuracy   |          |         |        |
   | Surface quality      |          |         |        |
   | Texture fidelity     |          |         |        |
   | Export format options |          |         |        |
   | Ease of use          |          |         |        |

---

## Real-World Challenge

### Reverse Engineering a Department Part

**Scenario**: Identify a broken, worn, or hard-to-source part in your department or workshop.

**Deliverable**: A complete reverse engineering workflow document.

1. **Identify the Part**
   - What is it? What does it do?
   - Why is it a candidate for reverse engineering? (Obsolete, long lead time, expensive to source)

2. **Document Current State**
   - Photograph the part from at least 4 angles.
   - Record all measurable dimensions.
   - Note material type and surface finish.

3. **Proposed Workflow**
   - Which AI tool(s) would you use and why?
   - What is the expected accuracy based on your guided exercise results?
   - What manual CAD work would be needed after AI processing?
   - What manufacturing method would you use for the replacement?

4. **Feasibility Assessment**
   - Estimated time: AI workflow vs. traditional manual measurement and CAD modeling.
   - Estimated cost: Tooling, material, labor.
   - Risk: What could go wrong? What is your fallback plan?

---

## Extension Task

### Research Presentation: Generative Design for Material Waste Reduction

**Question**: How could generative design reduce material waste in APC (Armored Personnel Carrier) operations, maintenance, and manufacturing?

**Requirements**:
- Research at least 3 real-world case studies of generative design in automotive, aerospace, or defense.
- Identify at least 2 APC components that could benefit from generative redesign.
- Estimate potential weight and material savings (use published case study percentages as benchmarks).
- Address: What infrastructure (software, printers, training) would be needed?
- Prepare a 5-minute presentation or 1-page summary.

**Suggested Research Sources**:
- Autodesk generative design case studies
- Airbus A320 partition bracket case study
- GM seat bracket generative redesign
- Published papers on topology optimization in defense applications
