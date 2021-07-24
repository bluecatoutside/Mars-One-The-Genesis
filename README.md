# Scene Definition

Using Blender projects, level of detail (LOD) is organized using a folder system. One level up uses a GLTF file export as an import to the Blender project at that level. E.g. kitchen_sink.gltf.

# Collision Definition

Hit boxes and (sometimes) meshes that resemble primitives are created. In practice, export the scene and the collision objects. A "diff" between exports of the scene without collision objects and the scene with collision objects will allow programs to identify collision objects. E.g. kitchen_sink.x3d is required to interpret kitchen_sink_C.x3d.

# File Type Overview

Overall, three file types are used.

* .GLTF file or the equivalent .GLB file.

* .BLEND file is the edited working document and why you need Github login credentials.

* .X3D file is the file containing the data for constructing a world for CANNON.js physics.