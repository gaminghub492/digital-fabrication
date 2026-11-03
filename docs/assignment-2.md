# Assignment 2 — Modular 3D Rocket

**Project:** Design and manufacture a detachable 3D-printed rocket kit  
**CAD software:** Onshape  
**Current progress:** CAD design and STL exports completed; physical printing and photographic evidence pending.

!!! info "Project status"
    I have completed the rocket model in Onshape and exported the individual Part Studio and assembled Assembly STL files. The physical 3D print has not yet been completed or documented. Print settings, photographs, and fit-test results will be added after manufacturing.

## 1. What was the goal?

The goal was to create a **modular rocket** as a three-dimensional CAD model and manufacture it using a 3D printer. The rocket needs to function as a **detachable kit** whose components can be assembled and removed. The teacher clarified that pins are not mandatory, provided the design remains detachable.

Another objective was to make the work reproducible by publishing the 3D source exports as a downloadable ZIP, together with a description of the design, manufacturing process, observations, and photographs of the printed result.

## 2. What did I do?

I designed the rocket in **Onshape**, separating the design into components rather than treating the entire object as a permanently fused part. I developed the rocket's main body geometry and connection features, and created assembled views to examine how the pieces fit together.

I exported **nine Part Studio STL files** and **two Assembly STL files**. These exports are included in the project's downloadable-file package, which will be published in the assets folder.

The STL files contain triangle meshes suitable for importing into slicer software. The assembly exports are useful for visualizing the assembled design; the individual part exports are more appropriate for planning detachable printing.

### Recorded STL exports

| File | Approximate bounding-box dimensions* | Purpose |
| --- | --- | --- |
| Part Studio 1.stl | 3.4 × 3.4 × 9.0 mm | Individual component |
| Part Studio 2.stl | 15.2 × 7.5 × 35.1 mm | Individual component |
| Part Studio 3.stl | 28.8 × 28.8 × 59.9 mm | Individual component |
| Part Studio 4.stl | 8.4 × 8.4 × 15.2 mm | Individual component |
| Part Studio 5.stl | 28.8 × 28.8 × 36.0 mm | Individual component |
| Part Studio 6.stl | 14.3 × 14.3 × 37.6 mm | Individual component |
| Part Studio 7.stl | 28.8 × 28.8 × 18.0 mm | Individual component |
| Part Studio 8.stl | 8.4 × 8.4 × 33.0 mm | Individual component |
| Part Studio 9.stl | 14.3 × 14.3 × 55.0 mm | Individual export requiring mesh review |
| Assembly 1.stl | 59.2 × 59.2 × 205.7 mm | Assembled export |
| Assembly 2.stl | 105.5 × 60.5 × 59.9 mm | Additional assembly export |

*Dimensions are measured from the STL mesh bounds, rounded to 0.1 mm. They describe each file's full extents, not necessarily the nominal CAD dimensions. They assume the exported coordinates are in millimeters.*

!!! warning "Mesh validation before printing"
    A preliminary mesh inspection found that **Part Studio 9.stl is not watertight**, and both assembled exports contain multiple shells or mesh irregularities. This alone does not prove the design is unprintable, but the affected models should be examined in slicer preview and repaired or re-exported if required. No successful test print has yet been confirmed.

## 3. What tools and materials did I use?

| Tool / material | Use |
| --- | --- |
| **Onshape** | CAD modeling and assembly construction |
| **STL** | Exporting geometric meshes for slicing and sharing |
| **GitHub** | Storing documentation and published project files |
| **MkDocs + Material** | Generating the documentation website |
| **GitHub Pages** | Making the project documentation publicly accessible |
| **3D printer and slicer** | To be identified and documented after printing |
| **Filament or resin** | To be recorded once the actual printer and material are known |

## 4. How does the detachable design work?

The rocket was designed as a multi-part kit. The geometry includes cylindrical connector features and separate structural sections. The intent is to allow the components to be fitted together and taken apart rather than printing the entire assembly as a single inseparable object.

The actual **fit, clearance, and ease of disassembly must be tested on the physical print**. A nominal match between a peg and a hole in CAD does not guarantee a functional fit after manufacturing: machine calibration, print orientation, and material behavior all affect the outcome.

## 5. What went wrong? What did I change?

**During CAD:** The design was divided into multiple models and assemblies so that connections and relative placement could be considered separately. Specific modeling failures or redesigns should be added here only if verified from the design history.

**During export review:** A preliminary mesh check highlighted an open or multi-shell export in `Part Studio 9.stl`. I will examine that file in the slicer or re-export it from Onshape if it causes a slicing error.

**During printing:** Not attempted or documented yet. I will record failed prints, dimensional mismatches, support issues, and any design revisions after testing.

## 6. Preparing the 3D print

Once the printer model is known, I will:

1. Select the exact printer and material profile in its slicer.
2. Import the **individual components** instead of attempting to print an already assembled model as one object.
3. Orient the parts for stability and manageable support removal.
4. Check scale, toolpaths, and small connection features in slicer preview.
5. Test a representative connection before printing the entire kit, if practical.
6. Print the components, remove supports, and test the assembly.

These are **planned actions**, not completed manufacturing results.

## 7. Open-source design files

I have exported the model as **11 STL files**: nine Part Studio exports and two Assembly exports. They have been collected into the ZIP archive **`Efe_Modular_Rocket_STL_Files.zip`**.

**File publication:** The ZIP has been prepared but still needs to be uploaded to this GitHub repository. After upload, this section will contain the direct download link. The STL files are mesh exports; an editable Onshape project link or STEP exports could also be added later for easier modification.

## 8. Photos of the printed rocket — to be added

!!! note "Photographs pending"
    Once the rocket is printed, I will add compressed photos here showing the separate printed pieces, the fully assembled rocket, and the connection details. Photos will only be described as completed evidence after they are actually taken.

Planned photo set:

- Individual parts arranged separately
- Rocket assembled
- Close-up of the detachable connections
- Any test prints, fit problems, or modifications

## 9. What was the result?

**Current result:** A completed digital rocket model in Onshape, with individual and assembled STL exports prepared for manufacturing and open-source sharing.

**Remaining result to document:** A successfully printed, detachable rocket and photographs demonstrating that its components can be assembled and removed.

The final manufacturing result, printer settings, and any fit adjustments will be recorded here after the physical print is complete.
