---
marp: true
theme: default
paginate: true
header: "Unit 5: From Pixels to Parts - AI in Engineering & CAD/CAM | APC AI Excellence Program"
footer: "Arab Potash Company | 2026"
---

# Unit 5: From Pixels to Parts
## AI in Engineering & CAD/CAM

**APC AI Excellence Program**

---

# Learning Objectives

By the end of this unit, you will be able to:

- **Distinguish** between artistic AI outputs and engineering-grade models
- **Use** Image-to-Mesh tools (Meshy, Luma AI, TripoSR) to generate 3D assets
- **Convert** raster images to scalable vectors using Vectorizer.ai
- **Apply** Generative Design in Fusion 360 for optimized part creation
- **Execute** a Reverse Engineering workflow using AI-assisted tools
- **Recognize** the limitations of current AI in engineering contexts

---

# Art vs Engineering: A Critical Distinction

| Aspect | Artistic 3D Output | Engineering-Grade Model |
|--------|-------------------|------------------------|
| **Purpose** | Visual appeal, rendering | Manufacturing, simulation |
| **Tolerance** | Approximate geometry | Precise dimensions (0.01mm+) |
| **Format** | OBJ, FBX (meshes) | STEP, IGES (parametric solids) |
| **Validation** | "Looks right" | FEA, stress analysis, GD&T |
| **Watertight** | Often not | Must be |

> **Key Insight:** AI-generated 3D models are a *starting point* for engineering, never a finished deliverable without human validation.

---

# The AI-Assisted Engineering Pipeline

```
Photo/Sketch --> AI Image-to-Mesh --> Raw 3D Mesh
                                          |
                                          v
                               Clean & Repair Mesh
                                          |
                                          v
                              Convert to Solid (CAD)
                                          |
                                          v
                          Engineering Validation (FEA/CFD)
                                          |
                                          v
                              Manufacturing Output (CAM)
```

- Each step requires **human expertise** and judgment
- AI accelerates the early stages dramatically

---

# Image-to-Mesh Tool: Meshy

**What it does:** Converts 2D images or text prompts into textured 3D meshes

- **Input:** Photo of a part, sketch, or text description
- **Output:** OBJ/FBX/GLB mesh with textures
- **Strengths:**
  - Fast turnaround (minutes, not hours)
  - Good for initial concept visualization
  - Texture generation included
- **Limitations:**
  - Non-parametric output (mesh only)
  - Geometry may not be dimensionally accurate
  - Internal features often missing

> **APC Use Case:** Quickly visualize a worn pump impeller from a maintenance photo before ordering replacement parts.

---

# Image-to-Mesh Tool: Luma AI & TripoSR

## Luma AI
- Specializes in **photogrammetry-style** 3D capture
- NeRF-based reconstruction from multiple photos
- Excellent for capturing **as-built conditions** of equipment

## TripoSR (by Stability AI)
- **Open-source** single-image 3D reconstruction
- Runs locally for sensitive/proprietary parts
- Fast inference (~0.5 seconds per model)

| Tool | Best For | Data Privacy | Cost |
|------|----------|-------------|------|
| Meshy | Text-to-3D concepts | Cloud-based | Subscription |
| Luma AI | Multi-photo reconstruction | Cloud-based | Freemium |
| TripoSR | Single-image, on-premise | Local/private | Free |

---

# Vectorizer.ai: Raster to Vector Conversion

**Problem:** Legacy engineering drawings exist only as scanned images (JPEG, PNG, TIFF)

**Solution:** Vectorizer.ai converts raster images to clean SVG/DXF vectors

- **How it works:**
  - AI identifies lines, curves, and shapes in raster images
  - Reconstructs them as mathematically precise vector paths
  - Preserves line weights and layer structure

- **Engineering Applications at APC:**
  - Digitize old P&ID diagrams from paper archives
  - Convert equipment photos to line drawings for documentation
  - Create scalable technical illustrations from screenshots

> **Tip:** Always verify converted dimensions against known references. AI vectorization is approximate.

---

# Generative Design in Fusion 360

**What is Generative Design?**
AI explores thousands of design alternatives based on your constraints.

**You define:**
- **Preserve geometry** - areas that must remain (mounting points, interfaces)
- **Obstacle geometry** - areas the design cannot occupy
- **Load cases** - forces, pressures, temperatures
- **Manufacturing method** - CNC, casting, 3D printing, etc.
- **Materials** - steel, aluminum, composites

**AI delivers:**
- Multiple optimized design options ranked by weight, stress, cost
- Organic shapes that outperform traditional designs
- Ready-to-manufacture geometry

> **APC Application:** Optimize custom brackets, supports, and fixtures used in potash processing equipment.

---

# Reverse Engineering Workflow with AI

**Scenario:** A critical legacy part has no drawings and the OEM no longer exists.

### Step-by-Step Workflow:

1. **Capture** - Photograph the part from multiple angles (or 3D scan)
2. **Reconstruct** - Use Luma AI / TripoSR to generate initial 3D mesh
3. **Clean** - Repair mesh in MeshLab or Blender (fill holes, smooth artifacts)
4. **Convert** - Import mesh into Fusion 360, convert to solid body
5. **Dimension** - Measure physical part with calipers; apply real dimensions to model
6. **Validate** - Compare AI model to physical measurements; iterate
7. **Document** - Generate engineering drawings with GD&T from final model

> **Critical:** Steps 5-7 are non-negotiable. AI gets you 60-70% of the way; engineering judgment completes the job.

---

# Limitations of AI in Engineering

- **Dimensional accuracy** - AI models lack real-world scale without reference
- **Internal features** - Holes, channels, threads are poorly captured from external images
- **Material properties** - AI cannot infer material grade, heat treatment, or coatings
- **Tolerances & fits** - No understanding of GD&T or mating requirements
- **Standards compliance** - Cannot verify ASME, ISO, or API standards
- **Liability** - AI-generated designs require PE stamp for critical applications

### The Golden Rule

> **AI is a powerful assistant, not a replacement for engineering judgment.** Every AI-generated model must be validated by a qualified engineer before use in production.

---

# Exercise 22: AI-Assisted Part Reconstruction

**Task:** Reverse-engineer a simple mechanical part using AI tools.

1. Select a non-critical part from your work area (bracket, cover, handle)
2. Take 4-6 photos from different angles
3. Upload to **Meshy** or **TripoSR** to generate a 3D mesh
4. Document the following in a report:
   - Quality of the AI-generated mesh vs. the real part
   - Features the AI captured well
   - Features the AI missed or got wrong
   - Estimated effort saved vs. manual CAD modeling

**Deliverable:** Comparison report with screenshots and measurements.

---

# Exercise 23: Generative Design Exploration

**Task:** Use Fusion 360 Generative Design on a real APC component.

1. Identify a bracket or support that could benefit from optimization
2. Define preserve/obstacle geometry and load cases
3. Run generative design study with at least 2 manufacturing methods
4. Compare results:

| Criteria | Original Design | AI Option A | AI Option B |
|----------|----------------|-------------|-------------|
| Weight | | | |
| Max Stress | | | |
| Manufacturability | | | |
| Estimated Cost | | | |

**Deliverable:** Design comparison table with recommendation and justification.

---

# Unit 5 Recap

| Topic | Key Takeaway |
|-------|-------------|
| Art vs Engineering | AI 3D output needs validation before engineering use |
| Image-to-Mesh | Meshy, Luma AI, TripoSR each serve different needs |
| Vectorizer.ai | Digitize legacy drawings, always verify dimensions |
| Generative Design | Define constraints; let AI explore the solution space |
| Reverse Engineering | AI accelerates capture; humans ensure accuracy |
| Limitations | No substitution for engineering judgment and standards |

> **Next Unit:** We explore Specialized AI Tools & Knowledge Engines for deeper research and knowledge management.

---

# Key Terms & Resources

- **Mesh vs. Solid** - Mesh is a surface approximation; solid is a mathematically complete volume
- **GD&T** - Geometric Dimensioning & Tolerancing (ASME Y14.5)
- **FEA** - Finite Element Analysis for stress/thermal simulation
- **NeRF** - Neural Radiance Fields (technology behind Luma AI)

**Tool Links:**
- Meshy: meshy.ai
- Luma AI: lumalabs.ai
- TripoSR: github.com/VAST-AI-Research/TripoSR
- Vectorizer.ai: vectorizer.ai
- Fusion 360: autodesk.com/fusion-360
