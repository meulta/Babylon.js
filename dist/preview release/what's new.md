- 2.3.0:
  - **Major updates**
    - Point lights shadow mapping. [Demo here](http://www.babylonjs-playground.com/#LYCSQ#12) ([deltakosh](https://github.com/deltakosh))
    - Introducing [Materials Library](https://github.com/BabylonJS/Babylon.js/tree/master/materialsLibrary) ([deltakosh](https://github.com/deltakosh))
      - Water material: http://doc.babylonjs.com/extensions/Water ([julien-moreau](https://github.com/julien-moreau))
      - Fire material: http://doc.babylonjs.com/extensions/fire ([julien-moreau](https://github.com/julien-moreau))
      - Normal material: http://doc.babylonjs.com/extensions/normal ([temechon](https://github.com/temechon))
      - Lava Material: http://doc.babylonjs.com/extensions/lava ([temechon](https://github.com/temechon))
      - PBR Material: http://doc.babylonjs.com/extensions/pbr ([deltakosh](https://github.com/deltakosh))
    - New cache mecanism for StandardMaterial ([deltakosh](https://github.com/deltakosh))
    - New Solid Particle System ([jerome](https://github.com/jbousquie))
    - New `StandardMaterial.lightmapTexture` which can be controlled with `StandardMaterial.useLightmapAsShadowMap` ([deltakosh](https://github.com/deltakosh))
    - Support for reflection probes. [See documentation here](http://doc.babylonjs.com/tutorials/How_to_use_Reflection_probes) ([deltakosh](https://github.com/deltakosh))
    - New serializers [folder](https://github.com/BabylonJS/Babylon.js/serializers) to host .babylon serializers ([deltakosh](https://github.com/deltakosh))
      - New .obj serializer ([BitOfGold](https://github.com/BitOfGold))
    - Sprites now can be [picked](http://www.babylonjs-playground.com/#1XMVZW#4) and can use [actions](http://www.babylonjs-playground.com/#9RUHH#4) ([deltakosh](https://github.com/deltakosh))
    - New `Mesh.CreatePolyhedron()` method ([jerome](https://github.com/jbousquie))
    - New `Mesh.CreateIcoSphere()` method. [Demo here](http://www.babylonjs-playground.com/#24DUYD) (G'kar)
    - Introducing [babylon.core.js](http://doc.babylonjs.com/generals/Framework_versions) ([deltakosh](https://github.com/deltakosh))
  - **Updates**
    - New button to log the camera position in the debug layer ([temechon](https://github.com/temechon))
    - Added `Animatable.goToFrame()` ([deltakosh](https://github.com/deltakosh))   
    - Fixed behavior or `Animation.CreateAndStartAnimation` and added `Animation.CreateMergeAndStartAnimation` to reproduce previous behavior ([deltakosh](https://github.com/deltakosh))
    - Adding `StandardMaterial.linkEmissiveWithDiffuse` to, well, link emissive with diffuse value. (With)[http://www.babylonjs-playground.com/#2FPUCS#2] and (without)[http://www.babylonjs-playground.com/#2FPUCS#1] ([deltakosh](https://github.com/deltakosh))
    - Adding support for equi-rectangular mapping. See [demo here](http://www.babylonjs-playground.com/#27FN5R#12) ([deltakosh](https://github.com/deltakosh))
    - Sprites and particles scheduler updated to be resolved before transparent objects ([deltakosh](https://github.com/deltakosh))
    - Added ability to deactivate ArcRotateCamera panning mechanism (by setting panningSensibility to 0) ([vouskprod](http://www.github.com/vousk))    
    - Added `DirectionalLight.autoUpdateExtends` to prevent directional lights to adapt to scene extends ([deltakosh](https://github.com/deltakosh))
    - Added a new parameter to `debugLayer.show()` to define root element to use ([deltakosh](https://github.com/deltakosh))
    - New `MeshBuilder` class used to create all kind of mesh shapes ([deltakosh](https://github.com/deltakosh))
    - Added `Scene.constantlyUpdateMeshUnderPointer` to improve performance when moving mouse ([deltakosh](https://github.com/deltakosh))
    - Added `StandardMaterial.disableLighting` ([deltakosh](https://github.com/deltakosh))
    - Improved reflection shader performance ([deltakosh](https://github.com/deltakosh))
    - New `Material.sideOrientation` property to define clockwise or counter-clockwise faces selection. [Demo here](http://www.babylonjs-playground.com/#1TZJQY) ([deltakosh](https://github.com/deltakosh))
    - It is now possible to create a custom loading screen. [PR](https://github.com/BabylonJS/Babylon.js/pull/700) ([RaananW](https://github.com/RaananW))
    - Per face color and texture feature in `MeshBuilder.CreateCylinder()` ([jerome](https://github.com/jbousquie))
    - _Arc_ feature in `CreateCylinder`, `CreateSphere`, `CreateTube`, `CreateDisc` and `CreateLathe` ([jerome](https://github.com/jbousquie))
    - _Slice_ feature in `MeshBuilder.CreateSphere()` ([jerome](https://github.com/jbousquie))
    - `closed` parameter in `MeshBuilder.CreateLathe()` ([jerome](https://github.com/jbousquie))
    - `diameter`, `hasRings`, `enclose` parameters in `MeshBuilder.CreateCreateCylinder()` ([jerome](https://github.com/jbousquie))
    - `Material.dispose()` now removes disposed material from meshes ([deltakosh](https://github.com/deltakosh))
    - New `Material.getBindedMeshes()` function ([deltakosh](https://github.com/deltakosh))
    - OimoJS Plugin now uses Quaternions exclusively and calculates body rotations correctly. [PR](https://github.com/BabylonJS/Babylon.js/pull/761) ([RaananW](https://github.com/RaananW))
    - It is now possible to get the physics engine's body and wolrd objects using the physics engine. [PR](https://github.com/BabylonJS/Babylon.js/pull/761) ([RaananW](https://github.com/RaananW))
    - new Heightmap Impostor for Cannon.js physics engine. [PR](https://github.com/BabylonJS/Babylon.js/pull/78), [Demo] (http://www.babylonjs-playground.com/#D3LQD#3) ([RaananW](https://github.com/RaananW))
    - A plane mesh can be created with a source plane (math). [PR](https://github.com/BabylonJS/Babylon.js/pull/779) ([RaananW](https://github.com/RaananW))
    - AbstractMesh.onPhysicsCollide will be triggered when a physics-enabled mesh collides against another. [PR](https://github.com/BabylonJS/Babylon.js/pull/806) ([RaananW](https://github.com/RaananW))
    - Added scene onPointerMove public callback. [PR](https://github.com/BabylonJS/Babylon.js/pull/810) ([RaananW](https://github.com/RaananW))
    - Added streaming support for BABYLON.Sound ([davrous](https://github.com/davrous))
    - Added collisionsEnabled and workerCollisions for serialization [PR](https://github.com/BabylonJS/Babylon.js/pull/830) ([Dad72](https://github.com/dad72))
  - **Bug fixes**
    - Fixed a bug with spherical mapping ([deltakosh](https://github.com/deltakosh)) 
    - Fixed a bug with clone and createInstance which was forcing the recomputation of bounding boxes ([deltakosh](https://github.com/deltakosh)) 
    - Fixed a bug with CSG when submeshes are kept ([deltakosh](https://github.com/deltakosh)) 
    - Fixed a bug with texture coordinates matrices ([deltakosh](https://github.com/deltakosh))
    - Fixed Sphere texture coordinates generation ([deltakosh](https://github.com/deltakosh))
    - Fixed a bug with `Mesh.attachToBone` when bone's matrix has a negative determinant ([deltakosh](https://github.com/deltakosh))
    - Fixed a possible but with the active camera while taking a screenshot. [PR](https://github.com/BabylonJS/Babylon.js/pull/701) ([RaananW](https://github.com/RaananW))
    - Fixed a bug with worker-collisions and instances. [PR](https://github.com/BabylonJS/Babylon.js/pull/705) ([RaananW](https://github.com/RaananW))
    - Fixed a bug with removed meshes and geometries from the worker-cache. [PR](https://github.com/BabylonJS/Babylon.js/pull/711) ([RaananW](https://github.com/RaananW))
    - Fixed `closePath` and `closeArray` ribbon parameter now working back together ([jerome](https://github.com/jbousquie))
    - Fixed morphing on capped tubes  ([jerome](https://github.com/jbousquie))
    - Fixed morphing on extruded shapes  ([jerome](https://github.com/jbousquie))
    - Fixed tube and extruded shape cap light artifact  ([jerome](https://github.com/jbousquie))
    - Fixed a bug calculating velocity during collision with gravity enabled. [PR](https://github.com/BabylonJS/Babylon.js/pull/738) ([RaananW](https://github.com/RaananW))
    - Fixed a bug in instance serialization. [PR](https://github.com/BabylonJS/Babylon.js/pull/726) ([RaananW](https://github.com/RaananW))
  - **Breaking changes**
    - `VertexData.CreateCylinder()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateRibbon()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateBox()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateSphere)` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateTorus()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateTorusKnot()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreatePlane()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateDisc()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateLines()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateDashedLines()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateGround()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateTiledGround()` now supports only the single _options_ parameter ([jerome](https://github.com/jbousquie))
    - `VertexData.CreateGroundFromHeightMap()` now supports only the single _options_ parameter ([deltakosh](https://github.com/deltakosh))
    - `Tools.IsExponantOfTwo()` renamed to `Tools.IsExponentOfTwo()` ([deltakosh](https://github.com/deltakosh))
    - `Tools.GetExponantOfTwo()` renamed to `Tools.GetExponentOfTwo()` ([deltakosh](https://github.com/deltakosh))
    - Updated Cannon.js plugin to the newest version (0.6.2). New cannon.js must be used. [PR](https://github.com/BabylonJS/Babylon.js/pull/755) ([RaananW](https://github.com/RaananW))