<div align="center">
  <!-- Light mode only logo -->
  <img src="logo.png#gh-light-mode-only" alt="logo" width="280" />   
  <!-- Dark mode only logo -->
  <img src="logo-dark-mode.png#gh-dark-mode-only" alt="logo" width="280" />
</div>

[![Version](https://img.shields.io/npm/v/@gsimone/zwei?style=flat&colorA=000000&colorB=000000)](https://www.npmjs.com/package/@gsimone/zwei)
[![Downloads](https://img.shields.io/npm/dt/@gsimone/zwei.svg?style=flat&colorA=000000&colorB=000000)](https://www.npmjs.com/package/@gsimone/zwei)
[![Discord Shield](https://img.shields.io/discord/740090768164651008?style=flat&colorA=000000&colorB=000000&label=discord&logo=discord&logoColor=ffffff)](https://discord.com/channels/740090768164651008/741751532592038022)
[![Open in GitHub Codespaces](https://img.shields.io/static/v1?&message=Open%20in%20%20Codespaces&style=flat&colorA=000000&colorB=000000&label=GitHub&logo=github&logoColor=ffffff)](https://github.com/codespaces/new?template_repository=pmndrs%2Fdrei)

A shrinking collection of useful helpers and simple ready-made abstractions for [@react-three/fiber](https://github.com/pmndrs/react-three-fiber). 

If you make a component that is generic enough to be useful to everyone, think about [CONTRIBUTING to Drei instead](https://github.com/pmndrs/drei/blob/master/CONTRIBUTING.md)!

```bash
npm install @gsimone/zwei
```

:point_right: this package is using the stand-alone [`three-stdlib`](https://github.com/pmndrs/three-stdlib) instead of [`three/examples/jsm`](https://github.com/mrdoob/three.js/tree/master/examples/jsm). :point_left:

### Basic usage:

```jsx
import { PerspectiveCamera, ... } from '@gsimone/zwei'
```

### React-native:

This fork does not support react-native.

### Index

<table>
  <tr>
    <td valign="top">
      <ul>
        <li><a href="#cameras">Cameras</a></li>
        <ul>
          <li><a href="#perspectivecamera">PerspectiveCamera</a></li>
          <li><a href="#orthographiccamera">OrthographicCamera</a></li>
          <li><a href="#cubecamera">CubeCamera</a></li>
        </ul>
        <li><a href="#controls">Controls</a></li>
        <ul>
          <li><a href="#cameracontrols">CameraControls</a></li>
        </ul>
        <li><a href="#abstractions">Abstractions</a></li>
        <ul>
          <li><a href="#image">Image</a></li>
          <li><a href="#text">Text</a></li>
          <li><a href="#text3d">Text3D</a></li>          
          <li><a href="#billboard">Billboard</a></li>
          <li><a href="#gradienttexture">GradientTexture</a></li>
          <li><a href="#edges">Edges</a></li>
          <li><a href="#outlines">Outlines</a></li>
          <li><a href="#trail">Trail</a></li>
          <li><a href="#sampler">Sampler</a></li>
          <li><a href="#computedattribute">Computed Attribute</a></li>
          <li><a href="#clone">Clone</a></li>
          <li><a href="#useanimations">useAnimations</a></li>
          <li><a href="#decal">Decal</a></li>
        </ul>
        <li><a href="#shaders">Shaders</a></li>
        <ul>
          <li><a href="#shadermaterial">shaderMaterial</a></li>
        </ul>
      </ul>
    </td>
    <td valign="top">
      <ul>
        <li><a href="#misc">Misc</a></li>
        <ul>
          <li><a href="#example">Example</a></li>
          <li><a href="#html">Html</a></li>
          <li><a href="#cycleraycast">CycleRaycast</a></li>
          <li><a href="#usedepthbuffer">useDepthBuffer</a></li>
          <li><a href="#usecontextbridge">useContextBridge</a></li>
          <li><a href="#usefbo">useFBO</a></li>
          <li><a href="#usecamera">useCamera</a></li>
          <li><a href="#usecubecamera">useCubeCamera</a></li>
          <li><a href="#usedetectgpu">useDetectGPU</a></li>          
          <li><a href="#useaspect">useAspect</a></li>
          <li><a href="#usecursor">useCursor</a></li>
          <li><a href="#useintersect">useIntersect</a></li>
          <li><a href="#useboxprojectedenv">useBoxProjectedEnv</a></li>
          <li><a href="#useTrail">useTrail</a></li>
          <li><a href="#useSurfaceSampler">useSurfaceSampler</a></li>
        </ul>
        <li><a href="#loading">Loaders</a></li>
        <ul>
          <li><a href="#useprogress">useProgress</a></li>
          <li><a href="#usegltf">useGLTF</a></li>
          <li><a href="#usefbx">useFBX</a></li>
          <li><a href="#usetexture">useTexture</a></li>
          <li><a href="#usecubetexture">useCubeTexture</a></li>
          <li><a href="#usevideotexture">useVideoTexture</a></li>
          <li><a href="#usetrailtexture">useTrailTexture</a></li>
          <li><a href="#usefont">useFont</a></li>
        </ul>
        <li><a href="#performance">Performance</a></li>
        <ul>
          <li><a href="#preload">Preload</a></li>
          <li><a href="#bakeshadows">BakeShadows</a></li>
          <li><a href="#meshbounds">meshBounds</a></li>
          <li><a href="#adaptivedpr">AdaptiveDpr</a></li>
          <li><a href="#adaptiveevents">AdaptiveEvents</a></li>
          <li><a href="#performancemonitor">PerformanceMonitor</a></li>          
        </ul>
      </ul>
    </td>
    <td valign="top">
      <ul>
        <li><a href="#shapes">Geometries</a></li>
        <ul>
          <li><a href="#roundedbox">RoundedBox</a></li>
          <li><a href="#screenquad">Screenquad</a></li>
        </ul>
        <li><a href="#staging">Staging</a></li>
        <ul>
          <li><a href="#center">Center</a></li>
          <li><a href="#resize">Resize</a></li>
          <li><a href="#BBAnchor">BBAnchor</a></li>        
          <li><a href="#bounds">Bounds</a></li>
          <li><a href="#environment">Environment</a></li>
          <li><a href="#useenvironment">useEnvironment</a></li>
          <li><a href="#usematcaptexture">useMatcapTexture</a></li>
          <li><a href="#usenormaltexture">useNormalTexture</a></li>
        </ul>
      </ul>
    </td>
  </tr>
</table>

# Cameras

#### PerspectiveCamera

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/camera-perspectivecamera--perspective-camera-scene-st)

```tsx
type Props = Omit<JSX.IntrinsicElements['perspectiveCamera'], 'children'> & {
  /** Registers the camera as the system default, fiber will start rendering with it */
  makeDefault?: boolean
  /** Making it manual will stop responsiveness and you have to calculate aspect ratio yourself. */
  manual?: boolean
  /** The contents will either follow the camera, or be hidden when filming if you pass a function */
  children?: React.ReactNode | ((texture: THREE.Texture) => React.ReactNode)
  /** Number of frames to render, 0 */
  frames?: number
  /** Resolution of the FBO, 256 */
  resolution?: number
  /** Optional environment map for functional use */
  envMap?: THREE.Texture
}
```

A responsive [THREE.PerspectiveCamera](https://threejs.org/docs/#api/en/cameras/PerspectiveCamera) that can set itself as the default.

```jsx
<PerspectiveCamera makeDefault {...props} />
<mesh />
```

You can also give it children, which will now occupy the same position as the camera and follow along as it moves.

```jsx
<PerspectiveCamera makeDefault {...props}>
  <mesh />
</PerspectiveCamera>
```

You can also drive it manually, it won't be responsive and you have to calculate aspect ratio yourself.

```jsx
<PerspectiveCamera manual aspect={...} onUpdate={(c) => c.updateProjectionMatrix()}>
```

You can use the PerspectiveCamera to film contents into a RenderTarget, similar to CubeCamera. As a child you must provide a render-function which receives the texture as its first argument. The result of that function will _not follow the camera_, instead it will be set invisible while the the FBO renders so as to avoid issues where the meshes that receive the texture are interrering.

```jsx
<PerspectiveCamera position={[0, 0, 10]}>
  {(texture) => (
    <mesh geometry={plane}>
      <meshBasicMaterial map={texture} />
    </mesh>
  )}
</PerspectiveCamera>
```

#### OrthographicCamera

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/camera-orthographiccamera--orthographic-camera-scene-st)

A responsive [THREE.OrthographicCamera](https://threejs.org/docs/#api/en/cameras/OrthographicCamera) that can set itself as the default.

```jsx
<OrthographicCamera makeDefault {...props}>
  <mesh />
</OrthographicCamera>
```

You can use the OrthographicCamera to film contents into a RenderTarget, it has the same API as PerspectiveCamera.

```jsx
<OrthographicCamera position={[0, 0, 10]}>
  {(texture) => (
    <mesh geometry={plane}>
      <meshBasicMaterial map={texture} />
    </mesh>
  )}
</OrthographicCamera>
```


# Controls

If available controls have damping enabled by default, they manage their own updates, remove themselves on unmount, are compatible with the `frameloop="demand"` canvas-flag. They inherit all props from their underlying [THREE controls](https://github.com/mrdoob/three.js/tree/master/examples/jsm/controls). They are the first effects to run before all other useFrames, to ensure that other components may mutate the camera on top of them.

[Some controls](https://github.com/search?q=repo%3Apmndrs%2Fdrei+language%3ATSX+path%3A%2F%5Esrc%5C%2Fcore%5C%2F.*Controls%5C.tsx%2F+makeDefault&type=code) allow you to set `makeDefault`, similar to, for instance, `PerspectiveCamera`. This will set [@react-three/fiber](https://docs.pmnd.rs/react-three-fiber/api/hooks#usethree)'s `controls` field in the root store. This can make it easier in situations where you want controls to be known and other parts of the app could respond to it. Some drei controls already take it into account, like `CameraShake`, `Gizmo` and `TransformControls`.

```tsx
<CameraControls makeDefault />
```

```tsx
const controls = useThree((state) => state.controls)
```

Drei currently exports OrbitControls [![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/controls-orbitcontrols--orbit-controls-story), MapControls [![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/controls-mapcontrols--map-controls-scene-st), TrackballControls, ArcballControls, FlyControls, DeviceOrientationControls, PointerLockControls [![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/controls-pointerlockcontrols--pointer-lock-controls-scene-st), FirstPersonControls [![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/controls-firstpersoncontrols--first-person-controls-story) CameraControls [![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/controls-cameracontrols--camera-controls-story) and FaceControls [![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/controls-facecontrols)

All controls react to the default camera. If you have a `<PerspectiveCamera makeDefault />` in your scene, they will control it. If you need to inject an imperative camera or one that isn't the default, use the `camera` prop: `<OrbitControls camera={MyCamera} />`.

PointerLockControls additionally supports a `selector` prop, which enables the binding of `click` event handlers for control activation to other elements than `document` (e.g. a 'Click here to play' button). All elements matching the `selector` prop will activate the controls. It will also center raycast events by default, so regular onPointerOver/etc events on meshes will continue to work.

#### CameraControls

<p>
  <a href="https://codesandbox.io/s/sew669"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/sew669/screenshot.png?v2" alt="CameraControls"/></a>
</p>

This is an implementation of the [camera-controls](https://github.com/yomotsu/camera-controls) library.

```tsx
<CameraControls />
```

```tsx
type CameraControlsProps = {
  /** The camera to control, default to the state's `camera` */
  camera?: PerspectiveCamera | OrthographicCamera
  /** DOM element to connect to, default to the state's `gl` renderer */
  domElement?: HTMLElement
  /** Reference this CameraControls instance as state's `controls` */
  makeDefault?: boolean
  /** Events callbacks, see: https://github.com/yomotsu/camera-controls#events */
  onStart?: (e?: { type: 'controlstart' }) => void
  onEnd?: (e?: { type: 'controlend' }) => void
  onChange?: (e?: { type: 'update' }) => void
}
```

# Gizmos

#### GizmoHelper

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/gizmos-gizmohelper--gizmo-helper-story)

Used by widgets that visualize and control camera position.

Two example gizmos are included: GizmoViewport and GizmoViewcube, and `useGizmoContext` makes it easy to create your own.

Make sure to set the `makeDefault` prop on your controls, in that case you do not have to define the onTarget and onUpdate props.

```jsx
<GizmoHelper
  alignment="bottom-right" // widget alignment within scene
  margin={[80, 80]} // widget margins (X, Y)
  onUpdate={/* called during camera animation  */}
  onTarget={/* return current camera target (e.g. from orbit controls) to center animation */}
  renderPriority={/* use renderPriority to prevent the helper from disappearing if there is another useFrame(..., 1)*/}
>
  <GizmoViewport axisColors={['red', 'green', 'blue']} labelColor="black" />
  {/* alternative: <GizmoViewcube /> */}
</GizmoHelper>
```

#### PivotControls

![](https://img.shields.io/badge/-Dom only-red)

<p>
  <a href="https://codesandbox.io/s/om2ff8"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/om2ff8/screenshot.png" alt="demo"/></a>
</p>

Controls for rotating and translating objects. These controls will stick to the object the transform and by offsetting or anchoring it forms a pivot. This control has HTML annotations for some transforms and supports `[tab]` for rounded values while dragging.

```tsx
type PivotControlsProps = {
  /** Scale of the gizmo, 1 */
  scale?: number
  /** Width of the gizmo lines, this is a THREE.Line2 prop, 2.5 */
  lineWidth?: number
  /** If fixed is true is remains constant in size, scale is now in pixels, false */
  fixed?: boolean
  /** Pivot does not act as a group, it won't shift contents but can offset in position */
  offset?: [number, number, number]
  /** Starting rotation */
  rotation?: [number, number, number]
  /** Starting matrix */
  matrix?: THREE.Matrix4
  /** Anchor point, like BBAnchor, each axis can be between -1/0/+1 */
  anchor?: [number, number, number]
  /** If autoTransform is true, automatically apply the local transform on drag, true */
  autoTransform?: boolean
  /** Allows you to switch individual axes off */
  activeAxes?: [boolean, boolean, boolean]
  /** RGB colors */
  axisColors?: [string | number, string | number, string | number]
  /** Color of the hovered item */
  hoveredColor?: string | number
  /** HTML value annotations, default: false */
  annotations?: boolean
  /** CSS Classname applied to the HTML annotations */
  annotationsClass?: string
  /** Drag start event */
  onDragStart?: () => void
  /** Drag event */
  onDrag?: (l: THREE.Matrix4, deltaL: THREE.Matrix4, w: THREE.Matrix4, deltaW: THREE.Matrix4) => void
  /** Drag end event */
  onDragEnd?: () => void
  /** Set this to false if you want the gizmo to be visible through faces */
  depthTest?: boolean
  opacity?: number
  visible?: boolean
  userData?: { [key: string]: any }
  children?: React.ReactNode
}
```

```jsx
<PivotControls>
  <mesh />
</PivotControls>
```

You can use Pivot as a controlled component, switch `autoTransform` off in that case and now you are responsible for applying the matrix transform yourself. You can also leave `autoTransform` on and apply the matrix to foreign objects, in that case Pivot will be able to control objects that are not parented within.

```jsx
const matrix = new THREE.Matrix4()
return (
  <PivotControls
    ref={ref}
    matrix={matrix}
    autoTransform={false}
    onDrag={({ matrix: matrix_ }) => matrix.copy(matrix_)}
```

#### TransformControls

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/gizmos-transformcontrols--transform-controls-story)

<p>
  <a href="https://codesandbox.io/s/btsbj"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/btsbj/screenshot.png" alt="Tranform controls"/></a>
</p>

An abstraction around [THREE.TransformControls](https://threejs.org/docs/#examples/en/controls/TransformControls).

You can wrap objects which then receive a transform gizmo.

```jsx
<TransformControls mode="translate">
  <mesh />
</TransformControls>
```

You could also reference the object which might make it easier to exchange the target. Now the object does not have to be part of the same sub-graph. References can be plain objects or React.MutableRefObjects.

```jsx
<TransformControls object={mesh} mode="translate" />
<mesh ref={mesh} />
```

If you are using other controls (Orbit, Trackball, etc), you will notice how they interfere, dragging one will affect the other. Default-controls will temporarily be disabled automatically when the user is pulling on the transform gizmo.

```jsx
<TransformControls mode="translate" />
<OrbitControls makeDefault />
```

#### Grid

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/gizmos-grid--use-grid-scene-st)

<p>
  <a href="https://codesandbox.io/s/19uq2u"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/19uq2u/screenshot.png" alt="Demo"/></a>
</p>

A y-up oriented, shader-based grid implementation.

```tsx
export type GridMaterialType = {
  /** Cell size, default: 0.5 */
  cellSize?: number
  /** Cell thickness, default: 0.5 */
  cellThickness?: number
  /** Cell color, default: black */
  cellColor?: THREE.ColorRepresentation
  /** Section size, default: 1 */
  sectionSize?: number
  /** Section thickness, default: 1 */
  sectionThickness?: number
  /** Section color, default: #2080ff */
  sectionColor?: THREE.ColorRepresentation
  /** Follow camera, default: false */
  followCamera?: boolean
  /** Display the grid infinitely, default: false */
  infiniteGrid?: boolean
  /** Fade distance, default: 100 */
  fadeDistance?: number
  /** Fade strength, default: 1 */
  fadeStrength?: number
}

export type GridProps = GridMaterialType & {
  /** Default plane-geometry arguments */
  args?: ConstructorParameters<typeof THREE.PlaneGeometry>
}
```

```jsx
<Grid />
```

#### useHelper

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/misc-usehelper--default-story)

A hook for a quick way to add helpers to existing nodes in the scene. It handles removal of the helper on unmount and auto-updates it by default.

```jsx
const mesh = useRef()
useHelper(mesh, BoxHelper, 'cyan')
useHelper(condition && mesh, BoxHelper, 'red') // you can pass false instead of the object ref to hide the helper

<mesh ref={mesh} ... />
```

# Shapes

#### Plane, Box, Sphere, Circle, Cone, Cylinder, Tube, Torus, TorusKnot, Ring, Tetrahedron, Polyhedron, Icosahedron, Octahedron, Dodecahedron, Extrude, Lathe, Shape

Short-cuts for a [mesh](https://threejs.org/docs/#api/en/objects/Mesh) with a [buffer geometry](https://threejs.org/docs/#api/en/core/BufferGeometry).

```jsx
<Box
  args={[1, 1, 1]}                // Args for the buffer geometry
  {...meshProps}                  // All THREE.Mesh props are valid
/>

// Plane with buffer geometry args
<Plane args={[2, 2]} />

// Box with color set on the default MeshBasicMaterial
<Box material-color="hotpink" />

// Sphere with a MeshStandardMaterial
<Sphere>
  <meshStandardMaterial color="hotpink" />
</Sphere>
```

#### RoundedBox

A box buffer geometry with rounded corners, done with extrusion.

```jsx
<RoundedBox
  args={[1, 1, 1]} // Width, height, depth. Default is [1, 1, 1]
  radius={0.05} // Radius of the rounded corners. Default is 0.05
  smoothness={4} // The number of curve segments. Default is 4
  bevelSegments={4} // The number of bevel segments. Default is 4, setting it to 0 removes the bevel, as a result the texture is applied to the whole geometry.
  creaseAngle={0.4} // Smooth normals everywhere except faces that meet at an angle greater than the crease angle
  {...meshProps} // All THREE.Mesh props are valid
>
  <meshPhongMaterial color="#f3f3f3" wireframe />
</RoundedBox>
```

#### ScreenQuad

```jsx
<ScreenQuad>
  <myMaterial />
</ScreenQuad>
```

A triangle that fills the screen, ideal for full-screen fragment shader work (raymarching, postprocessing).
👉 [Why a triangle?](https://www.cginternals.com/en/blog/2018-01-10-screen-aligned-quads-and-triangles.html)
👉 [Use as a post processing mesh](https://medium.com/@luruke/simple-postprocessing-in-three-js-91936ecadfb7)

#### Line

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/abstractions-line--basic-line)

Renders a THREE.Line2 or THREE.LineSegments2 (depending on the value of `segments`).

```jsx
<Line
  points={[[0, 0, 0], ...]}       // Array of points, Array<Vector3 | Vector2 | [number, number, number] | [number, number] | number>
  color="black"                   // Default
  lineWidth={1}                   // In pixels (default)
  segments                        // If true, renders a THREE.LineSegments2. Otherwise, renders a THREE.Line2
  dashed={false}                  // Default
  vertexColors={[[0, 0, 0], ...]} // Optional array of RGB values for each point
  {...lineProps}                  // All THREE.Line2 props are valid
  {...materialProps}              // All THREE.LineMaterial props are valid
/>
```

#### QuadraticBezierLine

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/abstractions-line--quadratic-bezier)

<p>
  <a href="https://codesandbox.io/s/2ij9u"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/2ij9u/screenshot.png" alt="Demo"/></a>
</p>

Renders a THREE.Line2 using THREE.QuadraticBezierCurve3 for interpolation.

```jsx
<QuadraticBezierLine
  start={[0, 0, 0]}               // Starting point, can be an array or a vec3
  end={[10, 0, 10]}               // Ending point, can be an array or a vec3
  mid={[5, 0, 5]}                 // Optional control point, can be an array or a vec3
  color="black"                   // Default
  lineWidth={1}                   // In pixels (default)
  dashed={false}                  // Default
  vertexColors={[[0, 0, 0], ...]} // Optional array of RGB values for each point
  {...lineProps}                  // All THREE.Line2 props are valid
  {...materialProps}              // All THREE.LineMaterial props are valid
/>
```

You can also update the line runtime.

```jsx
const ref = useRef()
useFrame((state) => {
  ref.current.setPoints(
    [0, 0, 0],
    [10, 0, 0],
    // [5, 0, 0] // Optional: mid-point
  )
}, [])
return <QuadraticBezierLine ref={ref} />
}
```

#### CubicBezierLine

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/abstractions-line--cubic-bezier)

Renders a THREE.Line2 using THREE.CubicBezierCurve3 for interpolation.

```jsx
<CubicBezierLine
  start={[0, 0, 0]}               // Starting point
  end={[10, 0, 10]}               // Ending point
  midA={[5, 0, 0]}                // First control point
  midB={[0, 0, 5]}                // Second control point
  color="black"                   // Default
  lineWidth={1}                   // In pixels (default)
  dashed={false}                  // Default
  vertexColors={[[0, 0, 0], ...]} // Optional array of RGB values for each point
  {...lineProps}                  // All THREE.Line2 props are valid
  {...materialProps}              // All THREE.LineMaterial props are valid
/>
```

#### CatmullRomLine

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/abstractions-line--catmull-rom)

Renders a THREE.Line2 using THREE.CatmullRomCurve3 for interpolation.

```jsx
<CatmullRomLine
  points={[[0, 0, 0], ...]}       // Array of Points
  closed={false}                  // Default
  curveType="centripetal"         // One of "centripetal" (default), "chordal", or "catmullrom"
  tension={0.5}                   // Default (only applies to "catmullrom" curveType)
  color="black"                   // Default
  lineWidth={1}                   // In pixels (default)
  dashed={false}                  // Default
  vertexColors={[[0, 0, 0], ...]} // Optional array of RGB values for each point
  {...lineProps}                  // All THREE.Line2 props are valid
  {...materialProps}              // All THREE.LineMaterial props are valid
/>
```

#### Facemesh

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/shapes-facemesh--facemesh-st)

Renders an oriented [MediaPipe face mesh](https://developers.google.com/mediapipe/solutions/vision/face_landmarker/web_js#handle_and_display_results):

```jsx
const faceLandmarkerResult = {
    "faceLandmarks": [
      [
        { "x": 0.5760777592658997, "y": 0.8639070391654968, "z": -0.030997956171631813 },
        { "x": 0.572094738483429, "y": 0.7886289358139038, "z": -0.07189624011516571 },
        // ...
      ],
      // ...
    ],
    "faceBlendshapes": [
      // ...
    ],
    "facialTransformationMatrixes": [
      // ...
    ]
  },
}
const points = faceLandmarkerResult.faceLandmarks[0]

<Facemesh points={points} />
```

```tsx
export type FacemeshProps = {
  /** an array of 468+ keypoints as returned by google/mediapipe tasks-vision, default: a sample face */
  points?: MediaPipePoints
  /** @deprecated an face object as returned by tensorflow/tfjs-models face-landmarks-detection */
  face?: MediaPipeFaceMesh
  /** constant width of the mesh, default: undefined */
  width?: number
  /** or constant height of the mesh, default: undefined */
  height?: number
  /** or constant depth of the mesh, default: 1 */
  depth?: number
  /** a landmarks tri supposed to be vertical, default: [159, 386, 200] (see: https://github.com/tensorflow/tfjs-models/tree/master/face-landmarks-detection#mediapipe-facemesh-keypoints) */
  verticalTri?: [number, number, number]
  /** a landmark index (to get the position from) or a vec3 to be the origin of the mesh. default: undefined (ie. the bbox center) */
  origin?: number | THREE.Vector3
  /** A facial transformation matrix, as returned by FaceLandmarkerResult.facialTransformationMatrixes (see: https://developers.google.com/mediapipe/solutions/vision/face_landmarker/web_js#handle_and_display_results) */
  facialTransformationMatrix?: (typeof FacemeshDatas.SAMPLE_FACELANDMARKER_RESULT.facialTransformationMatrixes)[0]
  /** Apply position offset extracted from `facialTransformationMatrix` */
  offset?: boolean
  /** Offset sensitivity factor, less is more sensible */
  offsetScalar?: number
  /** Fface blendshapes, as returned by FaceLandmarkerResult.faceBlendshapes (see: https://developers.google.com/mediapipe/solutions/vision/face_landmarker/web_js#handle_and_display_results) */
  faceBlendshapes?: (typeof FacemeshDatas.SAMPLE_FACELANDMARKER_RESULT.faceBlendshapes)[0]
  /** whether to enable eyes (nb. `faceBlendshapes` is required for), default: true */
  eyes?: boolean
  /** Force `origin` to be the middle of the 2 eyes (nb. `eyes` is required for), default: false */
  eyesAsOrigin?: boolean
  /** debug mode, default: false */
  debug?: boolean
}
```

Ref-api:

```tsx
const api = useRef<FacemeshApi>()

<Facemesh ref={api} points={points} />
```

```tsx
type FacemeshApi = {
  meshRef: React.RefObject<THREE.Mesh>
  outerRef: React.RefObject<THREE.Group>
  eyeRightRef: React.RefObject<FacemeshEyeApi>
  eyeLeftRef: React.RefObject<FacemeshEyeApi>
}
```

You can for example get face mesh world direction:

```tsx
api.meshRef.current.localToWorld(new THREE.Vector3(0, 0, -1))
```

or get L/R iris direction:

```tsx
api.eyeRightRef.current.irisDirRef.current.localToWorld(new THREE.Vector3(0, 0, -1))
```

# Abstractions

#### Image

<p>
  <a href="https://codesandbox.io/s/l4klb"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/l4klb/screenshot.png" alt="Horizontal tiles"/></a>
  <a href="https://codesandbox.io/s/gsm1y"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/gsm1y/screenshot.png" alt="useIntersect"/></a>
  <a href="https://codesandbox.io/s/x8gvs"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/x8gvs/screenshot.png" alt="Infinite scroll"/></a>
  <a href="https://codesandbox.io/s/yjhzv"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/yjhzv/screenshot.png" alt="Vertical scroll"/></a>
</p>

A shader-based image component with auto-cover (similar to css/background: cover).

```jsx
function Foo() {
  const ref = useRef()
  useFrame(() => {
    ref.current.material.zoom = ... // 1 and higher
    ref.current.material.grayscale = ... // between 0 and 1
    ref.current.material.color.set(...) // mix-in color
  })
  return <Image ref={ref} url="/file.jpg" />
}
```

To make the material transparent:

```jsx
<Image url="/file.jpg" transparent opacity={0.5} />
```

#### Text

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/abstractions-text--text-st) ![](https://img.shields.io/badge/-suspense-brightgreen)

<p>
  <a href="https://codesandbox.io/s/yup2o"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/yup2o/screenshot.png" alt="Demo"/></a>
</p>

Hi-quality text rendering w/ signed distance fields (SDF) and antialiasing, using [troika-3d-text](https://github.com/protectwise/troika/tree/master/packages/troika-3d-text). All of troikas props are valid! Text is suspense-based!

```jsx
<Text color="black" anchorX="center" anchorY="middle">
  hello world!
</Text>
```

Text will suspend while loading the font data, but in order to completely avoid FOUC you can pass the characters it needs to render.

```jsx
<Text font={fontUrl} characters="abcdefghijklmnopqrstuvwxyz0123456789!">
  hello world!
</Text>
```

#### Text3D

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/abstractions-text3d--text-3-d-st) ![](https://img.shields.io/badge/-suspense-brightgreen)

<p>
  <a href="https://codesandbox.io/s/x6obrb"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/x6obrb/screenshot.png" alt="Demo"/></a>
</p>

Render 3D text using ThreeJS's `TextGeometry`.

Text3D will suspend while loading the font data. Text3D requires fonts in JSON format generated through (typeface.json)[http://gero3.github.io/facetype.js], either as a path to a JSON file or a JSON object. If you face display issues try checking "Reverse font direction" in the typeface tool.

```jsx
<Text3D font={fontUrl} {...textOptions}>
  Hello world!
  <meshNormalMaterial />
</Text3D>
```

You can use any material. `textOptions` are options you'd pass to the `TextGeometry` constructor. Find more information about available options [here](https://threejs.org/docs/index.html?q=textg#examples/en/geometries/TextGeometry).

You can align the text using the `<Center>` component.

```jsx
<Center top left>
  <Text3D>hello</Text3D>
</Center>
```

It adds three properties that do not exist in the original `TextGeometry`, `lineHeight`, `letterSpacing` and smooth. LetterSpacing is a factor that is `1` by default. LineHeight is in threejs units and `0` by default. Smooth merges vertices with a tolerance and calls computeVertexNormals.

```jsx
<Text3D smooth={1} lineHeight={0.5} letterSpacing={-0.025}>{`hello\nworld`}</Text3D>
```

#### Effects

Abstraction around threes own [EffectComposer](https://threejs.org/docs/#examples/en/postprocessing/EffectComposer). By default it will prepend a render-pass and a gammacorrection-pass. Children are cloned, `attach` is given to them automatically. You can only use passes or effects in there.

By default it creates a render target with HalfFloatType, RGBAFormat. You can change all of this to your liking, inspect the types.

```jsx
import { SSAOPass } from "three-stdlib"

extend({ SSAOPass })

<Effects multisamping={8} renderIndex={1} disableGamma={false} disableRenderPass={false} disableRender={false}>
  <sSAOPass args={[scene, camera, 100, 100]} kernelRadius={1.2} kernelSize={0} />
</Effects>
```

#### PositionalAudio

<p>
  <a href="https://codesandbox.io/s/gkfhr"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/gkfhr/screenshot.png" alt="Demo"/></a>
</p>

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/abstractions-positionalaudio--positional-audio-scene-st) ![](https://img.shields.io/badge/-suspense-brightgreen)

A wrapper around [THREE.PositionalAudio](https://threejs.org/docs/#api/en/audio/PositionalAudio). Add this to groups or meshes to tie them to a sound that plays when the camera comes near.

```jsx
<PositionalAudio
  url="/sound.mp3"
  distance={1}
  loop
  {...props} // All THREE.PositionalAudio props are valid
/>
```

#### Billboard

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/abstractions-billboard--billboard-st)

Adds a `<group />` that always faces the camera.

```jsx
<Billboard
  follow={true}
  lockX={false}
  lockY={false}
  lockZ={false} // Lock the rotation on the z axis (default=false)
>
  <Text fontSize={1}>I'm a billboard</Text>
</Billboard>
```

#### ScreenSpace

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/abstractions-screenspace--screen-space-story)

Adds a `<group />` that aligns objects to screen space.

```jsx
<ScreenSpace
  depth={1} // Distance from camera
>
  <Box>I'm in screen space</Box>
</ScreenSpace>
```

#### GradientTexture

<p>
  <a href="https://codesandbox.io/s/l03yb"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/l03yb/screenshot.png" alt="Demo"/></a>
</p>

A declarative THREE.Texture which attaches to "map" by default. You can use this to create gradient backgrounds.

```jsx
<mesh>
  <planeGeometry />
  <meshBasicMaterial>
    <GradientTexture
      stops={[0, 1]} // As many stops as you want
      colors={['aquamarine', 'hotpink']} // Colors need to match the number of stops
      size={1024} // Size is optional, default = 1024
    />
  </meshBasicMaterial>
</mesh>
```

Radial gradient.

```jsx
import { GradientTexture, GradientType } from './GradientTexture'
;<mesh>
  <planeGeometry />
  <meshBasicMaterial>
    <GradientTexture
      stops={[0, 0.5, 1]} // As many stops as you want
      colors={['aquamarine', 'hotpink', 'yellow']} // Colors need to match the number of stops
      size={1024} // Size (height) is optional, default = 1024
      width={1024} // Width of the canvas producing the texture, default = 16
      type={GradientType.Radial} // The type of the gradient, default = GradientType.Linear
      innerCircleRadius={0} // Optional, the radius of the inner circle of the gradient, default = 0
      outerCircleRadius={'auto'} // Optional, the radius of the outer circle of the gradient, default = auto
    />
  </meshBasicMaterial>
</mesh>
```

#### Edges

<p>
  <a href="https://codesandbox.io/s/ny3p4"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/ny3p4/screenshot.png" alt="Demo"/></a>
</p>

Abstracts [THREE.EdgesGeometry](https://threejs.org/docs/#api/en/geometries/EdgesGeometry). It pulls the geometry automatically from its parent, optionally you can ungroup it and give it a `geometry` prop. You can give it children, for instance a custom material.

```jsx
<mesh>
  <boxGeometry />
  <meshBasicMaterial />
  <Edges
    scale={1.1}
    threshold={15} // Display edges only when the angle between two faces exceeds this value (default=15 degrees)
    color="white"
  />
</mesh>
```

#### Outlines

<p>
  <a href="https://codesandbox.io/s/2gh6jf"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/2gh6jf/screenshot.png" alt="Demo"/></a>
</p>

An ornamental component that extracts the geometry from its parent and displays an [inverted-hull outline](https://bnpr.gitbook.io/bnpr/outline/inverse-hull-method). Supported parents are `<mesh>`, `<skinnedMesh>` and `<instancedMesh>`.

```tsx
type OutlinesProps = JSX.IntrinsicElements['group'] & {
  /** Outline color, default: black */
  color: ReactThreeFiber.Color
  /** Line thickness is independent of zoom, default: false */
  screenspace: boolean
  /** Outline opacity, default: 1 */
  opacity: number
  /** Outline transparency, default: false */
  transparent: boolean
  /** Outline thickness, default 0.05 */
  thickness: number
  /** Geometry crease angle (0 === no crease), default: Math.PI */
  angle: number
}
```

```jsx
<mesh>
  <boxGeometry />
  <meshBasicMaterial />
  <Outlines thickness={0.05} color="hotpink" />
</mesh>
```

#### Trail

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/misc-trail--use-trail-st)

A declarative, `three.MeshLine` based Trails implementation. You can attach it to any mesh and it will give it a beautiful trail.

Props defined below with their default values.

```jsx
<Trail
  width={0.2} // Width of the line
  color={'hotpink'} // Color of the line
  length={1} // Length of the line
  decay={1} // How fast the line fades away
  local={false} // Wether to use the target's world or local positions
  stride={0} // Min distance between previous and current point
  interval={1} // Number of frames to wait before next calculation
  target={undefined} // Optional target. This object will produce the trail.
  attenuation={(width) => width} // A function to define the width in each point along it.
>
  {/* If `target` is not defined, Trail will use the first `Object3D` child as the target. */}
  <mesh>
    <sphereGeometry />
    <meshBasicMaterial />
  </mesh>

  {/* You can optionally define a custom meshLineMaterial to use. */}
  {/* <meshLineMaterial color={"red"} /> */}
</Trail>
```

👉 Inspired by [TheSpite's Codevember 2021 #9](https://spite.github.io/codevember-2021/9/)

#### Sampler

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/misc-sampler--sampler-st)

<p>
  <a href="https://codesandbox.io/s/ehflx3">
    <img width="20%" src="https://codesandbox.io/api/v1/sandboxes/ehflx3/screenshot.png" alt="Demo"/>
  </a> <br />
  <small>– <a href="https://codesandbox.io/s/ehflx3">Complex Demo</a> by <a href="https://twitter.com/CantBeFaraz">@CantBeFaraz</a></small> <br />
  <small>– <a href="https://codesandbox.io/s/k6rcp2">Simple Demo</a> by <a href="https://twitter.com/ggsimm">@ggsimm</a></small>
</p>

Declarative abstraction around MeshSurfaceSampler & InstancedMesh.
It samples points from the passed mesh and transforms an InstancedMesh's matrix to distribute instances on the points.

Check the demos & code for more.

You can either pass a Mesh and InstancedMesh as children:

```tsx
// This simple example scatters 1000 spheres on the surface of the sphere mesh.
<Sampler
  weight={'normal'} // the name of the attribute to be used as sampling weight
  transform={transformPoint} // a function that transforms each instance given a sample. See the examples for more.
  count={16} // Number of samples
>
  <mesh>
    <sphereGeometry args={[2]} />
  </mesh>

  <instancedMesh args={[null, null, 1_000]}>
    <sphereGeometry args={[0.1]} />
  </instancedMesh>
</Sampler>
```

or use refs when you can't compose declaratively:

```tsx
const { nodes } = useGLTF('my/mesh/url')
const mesh = useRef(nodes)
const instances = useRef()

return <>
  <instancedMesh args={[null, null, 1_000]}>
    <sphereGeometry args={[0.1]}>
  </instancedMesh>

  <Sampler mesh={mesh} instances={instances}>
</>
```


#### Clone

<p>
  <a href="https://codesandbox.io/s/42glz0"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/42glz0/screenshot.png" alt="Demo"/></a>
</p>

Declarative abstraction around THREE.Object3D.clone. This is useful when you want to create a shallow copy of an existing fragment (and Object3D, Groups, etc) into your scene, for instance a group from a loaded GLTF. This clone is now re-usable, but it will still refer to the original geometries and materials.

```ts
<Clone
  /** Any pre-existing THREE.Object3D (groups, meshes, ...), or an array of objects */
  object: THREE.Object3D | THREE.Object3D[]
  /** Children will be placed within the object, or within the group that holds arrayed objects */
  children?: React.ReactNode
  /** Can clone materials and/or geometries deeply (default: false) */
  deep?: boolean | 'materialsOnly' | 'geometriesOnly'
  /** The property keys it will shallow-clone (material, geometry, visible, ...) */
  keys?: string[]
  /** Can either spread over props or fill in JSX children, applies to every mesh within */
  inject?: MeshProps | React.ReactNode | ((object: THREE.Object3D) => React.ReactNode)
  /** Short access castShadow, applied to every mesh within */
  castShadow?: boolean
  /** Short access receiveShadow, applied to every mesh within */
  receiveShadow?: boolean
/>
```

You create a shallow clone by passing a pre-existing object to the `object` prop.

```jsx
const { nodes } = useGLTF(url)
return (
  <Clone object={nodes.table} />
```

Or, multiple objects:

```jsx
<Clone object={[nodes.foo, nodes.bar]} />
```

You can dynamically insert objects, these will apply to anything that isn't a group or a plain object3d (meshes, lines, etc):

```jsx
<Clone object={nodes.table} inject={<meshStandardMaterial color="green" />} />
```

Or make inserts conditional:

```jsx
<Clone object={nodes.table} inject={
  {(object) => (object.name === 'table' ? <meshStandardMaterial color="green" /> : null)}
} />
```

#### useAnimations

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/abstractions-useanimations--use-animations-st)

<p>
  <a href="https://codesandbox.io/s/pecl6"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/pecl6/screenshot.png" alt="Demo"/></a>
</p>

A hook that abstracts [AnimationMixer](https://threejs.org/docs/#api/en/animation/AnimationMixer).

```jsx
const { nodes, materials, animations } = useGLTF(url)
const { ref, mixer, names, actions, clips } = useAnimations(animations)
useEffect(() => {
  actions?.jump.play()
})
return (
  <mesh ref={ref} />
```

The hook can also take a pre-existing root (which can be a plain object3d or a reference to one):

```jsx
const { scene, animations } = useGLTF(url)
const { actions } = useAnimations(animations, scene)
return <primitive object={scene} />
```

#### MarchingCubes

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/abstractions-marchingcubes--marching-cubes-story)

An abstraction for threes [MarchingCubes](https://threejs.org/examples/#webgl_marchingcubes)

```jsx
<MarchingCubes resolution={50} maxPolyCount={20000} enableUvs={false} enableColors={true}>
  <MarchingCube strength={0.5} subtract={12} color={new Color('#f0f')} position={[0.5, 0.5, 0.5]} />

  <MarchingPlane planeType="y" strength={0.5} subtract={12} />
</MarchingCubes>
```

#### Decal

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/misc-decal--decal-st)

<p>
  <a href="https://codesandbox.io/s/ymb5d9"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/ymb5d9/screenshot.png" alt="Demo"/></a>
</p>

Abstraction around Three's `DecalGeometry`. It will use the its parent `mesh` as the decal surface by default.

The decal box has to intersect the surface, otherwise it will not be visible. if you do not specifiy a rotation it will look at the parents center point. You can also pass a single number as the rotation which allows you to spin it.

```js
<mesh>
  <sphereGeometry />
  <meshBasicMaterial />
  <Decal
    debug // Makes "bounding box" of the decal visible
    position={[0, 0, 0]} // Position of the decal
    rotation={[0, 0, 0]} // Rotation of the decal (can be a vector or a degree in radians)
    scale={1} // Scale of the decal
    polygonOffset
    polygonOffsetFactor={-1} // The mesh should take precedence over the original
  >
    <meshBasicMaterial map={texture} />
  </Decal>
</mesh>
```

If you do not specify a material it will create a transparent meshBasicMaterial with a polygonOffsetFactor of -10.

```jsx
<mesh>
  <sphereGeometry />
  <meshBasicMaterial />
  <Decal map={texture} />
</mesh>
```

If declarative composition is not possible, use the `mesh` prop to define the surface the decal must attach to.

```js
<Decal mesh={ref}>
  <meshBasicMaterial map={texture} polygonOffset polygonOffsetFactor={-1} />
</Decal>
```

#### Svg

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/abstractions-svg--svg-st)

Wrapper around the `three` [svg loader](https://threejs.org/examples/?q=sv#webgl_loader_svg) demo.

Accepts an SVG url or svg raw data.

```js
<Svg src={urlOrRawSvgString} />
```

#### Gltf

This is a convenience component that will load a gltf file and clone the scene using [drei/Clone](#clone). That means you can re-use and mount the same gltf file multiple times. It accepts all props that Clone does, including shortcuts (castShadow, receiveShadow) and material overrides.

```js
<Gltf src="/model.glb" receiveShadow castShadow />
```

#### AsciiRenderer

<p>
  <a href="https://codesandbox.io/s/vq9wsl"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/vq9wsl/screenshot.png" alt="Demo"/></a>
</p>

Abstraction of three's [AsciiEffect](https://threejs.org/examples/?q=as#webgl_effects_ascii). It creates a DOM layer on top of the canvas and renders the scene as ascii characters.

```tsx
type AsciiRendererProps = {
  /** Render index, default: 1 */
  renderIndex?: number
  /** CSS background color (can be "transparent"), default: black */
  bgColor?: string
  /** CSS character color, default: white */
  fgColor?: string
  /** Characters, default: ' .:-+*=%@#' */
  characters?: string
  /** Invert character, default: true */
  invert?: boolean
  /** Colorize output (very expensive!), default: false */
  color?: boolean
  /** Level of detail, default: 0.15 */
  resolution?: number
}
```

```jsx
<Canvas>
  <AsciiRenderer />
```

# Shaders

#### MeshReflectorMaterial

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/shaders-meshreflectormaterial--reflector-st)

<p>
  <a href="https://codesandbox.io/s/lx2h8"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/lx2h8/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/l900i"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/l900i/screenshot.png" alt="Demo"/></a>
</p>

Easily add reflections and/or blur to any mesh. It takes surface roughness into account for a more realistic effect. This material extends from [THREE.MeshStandardMaterial](https://threejs.org/docs/#api/en/materials/MeshStandardMaterial) and accepts all its props.

```jsx
<mesh>
  <planeGeometry />
  <MeshReflectorMaterial
    blur={[0, 0]} // Blur ground reflections (width, height), 0 skips blur
    mixBlur={0} // How much blur mixes with surface roughness (default = 1)
    mixStrength={1} // Strength of the reflections
    mixContrast={1} // Contrast of the reflections
    resolution={256} // Off-buffer resolution, lower=faster, higher=better quality, slower
    mirror={0} // Mirror environment, 0 = texture colors, 1 = pick up env colors
    depthScale={0} // Scale the depth factor (0 = no depth, default = 0)
    minDepthThreshold={0.9} // Lower edge for the depthTexture interpolation (default = 0)
    maxDepthThreshold={1} // Upper edge for the depthTexture interpolation (default = 0)
    depthToBlurRatioBias={0.25} // Adds a bias factor to the depthTexture before calculating the blur amount [blurFactor = blurTexture * (depthTexture + bias)]. It accepts values between 0 and 1, default is 0.25. An amount > 0 of bias makes sure that the blurTexture is not too sharp because of the multiplication with the depthTexture
    distortion={1} // Amount of distortion based on the distortionMap texture
    distortionMap={distortionTexture} // The red channel of this texture is used as the distortion map. Default is null
    debug={0} /* Depending on the assigned value, one of the following channels is shown:
      0 = no debug
      1 = depth channel
      2 = base channel
      3 = distortion channel
      4 = lod channel (based on the roughness)
    */
    reflectorOffset={0.2} // Offsets the virtual camera that projects the reflection. Useful when the reflective surface is some distance from the object's origin (default = 0)
  />
</mesh>
```

#### MeshWobbleMaterial

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/shaders-meshwobblematerial--mesh-wobble-material-st)

This material makes your geometry wobble and wave around. It was taken from the [threejs-examples](https://threejs.org/examples/#webgl_materials_modified) and adapted into a self-contained material.

```jsx
<mesh>
  <boxGeometry />
  <MeshWobbleMaterial factor={1} speed={10} />
</mesh>
```

#### MeshDistortMaterial

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/shaders-meshdistortmaterial--mesh-distort-material-st)

<p>
  <a href="https://codesandbox.io/s/l03yb"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/l03yb/screenshot.png" alt="Demo"/></a>
</p>

This material makes your geometry distort following simplex noise.

```jsx
<mesh>
  <boxGeometry />
  <MeshDistortMaterial distort={1} speed={10} />
</mesh>
```

#### MeshRefractionMaterial

<p>
  <a href="https://codesandbox.io/s/zqrreo"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/zqrreo/screenshot.png" alt="Demo"/></a>
</p>

A convincing Glass/Diamond refraction material.

```tsx
type MeshRefractionMaterialProps = JSX.IntrinsicElements['shaderMaterial'] & {
  /** Environment map */
  envMap: THREE.CubeTexture | THREE.Texture
  /** Number of ray-cast bounces, it can be expensive to have too many, 2 */
  bounces?: number
  /** Refraction index, 2.4 */
  ior?: number
  /** Fresnel (strip light), 0 */
  fresnel?: number
  /** RGB shift intensity, can be expensive, 0 */
  aberrationStrength?: number
  /** Color, white */
  color?: ReactThreeFiber.Color
  /** If this is on it uses fewer ray casts for the RGB shift sacrificing physical accuracy, true */
  fastChroma?: boolean
}
```

If you want it to reflect other objects in the scene you best pair it with a cube-camera.

```jsx
<CubeCamera>
  {(texture) => (
    <mesh geometry={diamondGeometry} {...props}>
      <MeshRefractionMaterial envMap={texture} />
    </mesh>
  )}
</CubeCamera>
```

Otherwise just pass it an environment map.

```jsx
const texture = useLoader(RGBELoader, "/textures/royal_esplanade_1k.hdr")
return (
  <mesh geometry={diamondGeometry} {...props}>
    <MeshRefractionMaterial envMap={texture} />
```

#### MeshTransmissionMaterial

<p>
  <a href="https://codesandbox.io/s/hmgdjq"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/hmgdjq/screenshot.png" alt="Demo"/></a>
</p>

An improved THREE.MeshPhysicalMaterial. It acts like a normal PhysicalMaterial in terms of transmission support, thickness, ior, roughness, etc., but has chromatic aberration, noise-based roughness blur, (primitive) anisotropic blur support, and unlike the original it can "see" other transmissive or transparent objects which leads to improved visuals.

Although it should be faster than MPM keep in mind that it can still be expensive as it causes an additional render pass of the scene. Low samples and low resolution will make it faster. If you use roughness consider using a tiny resolution, for instance 32x32 pixels, it will still look good but perform much faster.

For performance and visual reasons the host mesh gets removed from the render-stack temporarily. If you have other objects that you don't want to see reflected in the material just add them to the parent mesh as children.

```tsx
type MeshTransmissionMaterialProps = JSX.IntrinsicElements['meshPhysicalMaterial'] & {
  /* Transmission, default: 1 */
  transmission?: number
  /* Thickness (refraction), default: 0 */
  thickness?: number
  /** Backside thickness (when backside is true), default: 0 */
  backsideThickness?: number
  /* Roughness (blur), default: 0 */
  roughness?: number
  /* Chromatic aberration, default: 0.03 */
  chromaticAberration?: number
  /* Anisotropy, default: 0.1 */
  anisotropicBlur?: number
  /* Distortion, default: 0 */
  distortion?: number
  /* Distortion scale, default: 0.5 */
  distortionScale: number
  /* Temporal distortion (speed of movement), default: 0.0 */
  temporalDistortion: number
  /** The scene rendered into a texture (use it to share a texture between materials), default: null  */
  buffer?: THREE.Texture
  /** transmissionSampler, you can use the threejs transmission sampler texture that is
   *  generated once for all transmissive materials. The upside is that it can be faster if you
   *  use multiple MeshPhysical and Transmission materials, the downside is that transmissive materials
   *  using this can't see other transparent or transmissive objects nor do you have control over the
   *  buffer and its resolution, default: false */
  transmissionSampler?: boolean
  /** Render the backside of the material (more cost, better results), default: false */
  backside?: boolean
  /** Resolution of the local buffer, default: undefined (fullscreen) */
  resolution?: number
  /** Resolution of the local buffer for backfaces, default: undefined (fullscreen) */
  backsideResolution?: number
  /** Refraction samples, default: 6 */
  samples?: number
  /** Buffer scene background (can be a texture, a cubetexture or a color), default: null */
  background?: THREE.Texture
}
```

```jsx
return (
  <mesh geometry={geometry} {...props}>
    <MeshTransmissionMaterial />
```

If each material rendering the scene on its own is too expensive you can share a buffer texture. Either by enabling `transmissionSampler` which would use the threejs-internal buffer that MeshPhysicalMaterials use. This might be faster, the downside is that no transmissive material can "see" other transparent or transmissive objects.

```jsx
<mesh geometry={torus}>
  <MeshTransmissionMaterial transmissionSampler />
</mesh>
<mesh geometry={sphere}>
  <MeshTransmissionMaterial transmissionSampler />
</mesh>
```

Or, by passing a texture to `buffer` manually, for instance using useFBO.

```jsx
const buffer = useFBO()
useFrame((state) => {
  state.gl.setRenderTarget(buffer)
  state.gl.render(state.scene, state.camera)
  state.gl.setRenderTarget(null)
})
return (
  <>
    <mesh geometry={torus}>
      <MeshTransmissionMaterial buffer={buffer.texture} />
    </mesh>
    <mesh geometry={sphere}>
      <MeshTransmissionMaterial buffer={buffer.texture} />
    </mesh>
```

Or a PerspectiveCamera.

```jsx
<PerspectiveCamera makeDefault fov={75} position={[10, 0, 15]} resolution={1024}>
  {(texture) => (
    <>
      <mesh geometry={torus}>
        <MeshTransmissionMaterial buffer={texture} />
      </mesh>
      <mesh geometry={sphere}>
        <MeshTransmissionMaterial buffer={texture} />
      </mesh>
    </>
  )}
```

This would mimic the default MeshPhysicalMaterial behaviour, these materials won't "see" one another, but at least they would pick up on everything else, including transmissive or transparent objects.

#### MeshDiscardMaterial

A material that renders nothing. In comparison to `<mesh visible={false}` it can be used to hide objects from the scene while still displays shadows and children.

```jsx
<mesh castShadow>
  <torusKnotGeonetry />
  <MeshDiscardMaterial />
  {/* Shadows and edges will show, but the model itself won't */}
  <Edges />
```

#### PointMaterial

<p>
  <a href="https://codesandbox.io/s/eq7sc"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/eq7sc/screenshot.png" alt="Demo"/></a>
</p>

Antialiased round dots. It takes the same props as regular [THREE.PointsMaterial](https://threejs.org/docs/index.html?q=PointsMaterial#api/en/materials/PointsMaterial) on which it is based.

```jsx
<points>
  <PointMaterial transparent vertexColors size={15} sizeAttenuation={false} depthWrite={false} />
</points>
```

#### SoftShadows

<p>
  <a href="https://codesandbox.io/s/ykfpwf"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/ykfpwf/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/dh2jc"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/dh2jc/screenshot.png" alt="Demo"/></a>
</p>

```tsx
type SoftShadowsProps = {
  /** Size of the light source (the larger the softer the light), default: 25 */
  size?: number
  /** Number of samples (more samples less noise but more expensive), default: 10 */
  samples?: number
  /** Depth focus, use it to shift the focal point (where the shadow is the sharpest), default: 0 (the beginning) */
  focus?: number
}
```

Injects percent closer soft shadows (pcss) into threes shader chunk. Mounting and unmounting this component will lead to all shaders being be re-compiled, although it will only cause overhead if SoftShadows is mounted after the scene has already rendered, if it mounts with everything else in your scene shaders will compile naturally.

```jsx
<SoftShadows />
```

#### shaderMaterial

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/shaders-shadermaterial--shader-material-story)

<p>
  <a href="https://codesandbox.io/s/ni6v4"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/ni6v4/screenshot.png" alt="Demo"/></a>
</p>

Creates a THREE.ShaderMaterial for you with easier handling of uniforms, which are automatically declared as setter/getters on the object and allowed as constructor arguments.

```jsx
import { extend } from '@react-three/fiber'

const ColorShiftMaterial = shaderMaterial(
  { time: 0, color: new THREE.Color(0.2, 0.0, 0.1) },
  // vertex shader
  /*glsl*/`
    varying vec2 vUv;
    void main() {
      vUv = uv;
      gl_Position = projectionMatrix * modelViewMatrix * vec4(position, 1.0);
    }
  `,
  // fragment shader
  /*glsl*/`
    uniform float time;
    uniform vec3 color;
    varying vec2 vUv;
    void main() {
      gl_FragColor.rgba = vec4(0.5 + 0.3 * sin(vUv.yxx + time) + color, 1.0);
    }
  `
)

// declaratively
extend({ ColorShiftMaterial })
...
<mesh>
  <colorShiftMaterial color="hotpink" time={1} />
</mesh>

// imperatively, all uniforms are available as setter/getters and constructor args
const material = new ColorShiftMaterial({ color: new THREE.Color("hotpink") })
material.time = 1
```

`shaderMaterial` attaches a unique `key` property to the prototype class. If you wire it to Reacts own `key` property, you can enable hot-reload.

```jsx
import { ColorShiftMaterial } from './ColorShiftMaterial'

extend({ ColorShiftMaterial })

// in your component
<colorShiftMaterial key={ColorShiftMaterial.key} color="hotpink" time={1} />
```

# Modifiers

#### CurveModifier

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/modifiers-curvemodifier)

Given a curve will replace the children of this component with a mesh that move along said curve calling the property `moveAlongCurve` on the passed ref. Uses [three's Curve Modifier](https://threejs.org/examples/#webgl_modifier_curve)

```jsx
const curveRef = useRef()

const curve = React.useMemo(() => new THREE.CatmullRomCurve3([...handlePos], true, 'centripetal'), [handlePos])

return (
  <CurveModifier ref={curveRef} curve={curve}>
    <mesh>
      <boxGeometry args={[10, 10]} />
    </mesh>
  </CurveModifier>
)
```

# Misc

#### useContextBridge

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/misc-usecontextbridge--use-context-bridge-st)

Allows you to forward contexts provided above the `<Canvas />` to be consumed from within the `<Canvas />` normally

```jsx
function SceneWrapper() {
  // bridge any number of contexts
  // Note: These contexts must be provided by something above this SceneWrapper component
  //       You cannot render the providers for these contexts inside this component
  const ContextBridge = useContextBridge(ThemeContext, GreetingContext)
  return (
    <Canvas>
      <ContextBridge>
        <Scene />
      </ContextBridge>
    </Canvas>
  )
}

function Scene() {
  // we can now consume a context within the Canvas
  const theme = React.useContext(ThemeContext)
  const greeting = React.useContext(GreetingContext)
  return (
    //...
  )
}
```

#### Example

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/misc-example--example-st)

> **Warning** solely for [`CONTRIBUTING`](CONTRIBUTING.md#example) purposes

A "counter" example.

```tsx
<Example font="/Inter_Bold.json" />
```

```tsx
type ExampleProps = {
  font: string
  color?: Color
  debug?: boolean
  bevelSize?: number
}
```

Ref-api:

```tsx
const api = useRef<ExampleApi>()

<Example ref={api} font="/Inter_Bold.json" />
```

```tsx
type ExampleApi = {
  incr: (x?: number) => void
  decr: (x?: number) => void
}
```

#### Html

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/misc-html--html-st) ![](https://img.shields.io/badge/-Dom only-red)

<p>
  <a href="https://codesandbox.io/s/0n9it"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/0n9it/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/qyz5r"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/qyz5r/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/9keg6"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/9keg6/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/6oei7"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/6oei7/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/wp9mkp"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/wp9mkp/screenshot.png" alt="demo"/></a>
</p>

Allows you to tie HTML content to any object of your scene. It will be projected to the objects whereabouts automatically.

```jsx
<Html
  as='div' // Wrapping element (default: 'div')
  wrapperClass // The className of the wrapping element (default: undefined)
  prepend // Project content behind the canvas (default: false)
  center // Adds a -50%/-50% css transform (default: false) [ignored in transform mode]
  fullscreen // Aligns to the upper-left corner, fills the screen (default:false) [ignored in transform mode]
  distanceFactor={10} // If set (default: undefined), children will be scaled by this factor, and also by distance to a PerspectiveCamera / zoom by a OrthographicCamera.
  zIndexRange={[100, 0]} // Z-order range (default=[16777271, 0])
  portal={domnodeRef} // Reference to target container (default=undefined)
  transform // If true, applies matrix3d transformations (default=false)
  sprite // Renders as sprite, but only in transform mode (default=false)
  calculatePosition={(el: Object3D, camera: Camera, size: { width: number; height: number }) => number[]} // Override default positioning function. (default=undefined) [ignored in transform mode]
  occlude={[ref]} // Can be true or a Ref<Object3D>[], true occludes the entire scene (default: undefined)
  onOcclude={(visible) => null} // Callback when the visibility changes (default: undefined)
  {...groupProps} // All THREE.Group props are valid
  {...divProps} // All HTMLDivElement props are valid
>
  <h1>hello</h1>
  <p>world</p>
</Html>
```

Html can hide behind geometry using the `occlude` prop.

```jsx
<Html occlude />
```

When the Html object hides it sets the opacity prop on the innermost div. If you want to animate or control the transition yourself then you can use `onOcclude`.

```jsx
const [hidden, set] = useState()

<Html
  occlude
  onOcclude={set}
  style={{
    transition: 'all 0.5s',
    opacity: hidden ? 0 : 1,
    transform: `scale(${hidden ? 0.5 : 1})`
  }}
/>
```

**Blending occlusion**

Html can hide behind geometry as if it was part of the 3D scene using this mode. It can be enabled by using `"blending"` as the `occlude` prop.

```jsx
// Enable real occlusion
<Html occlude="blending" />
```

You can also give HTML material properties using the `material` prop.

```jsx
<Html
  occlude
  material={
    <meshPhysicalMaterial
      side={DoubleSide} // Required
      opacity={0.1} // Degree of influence of lighting on the HTML
      ... // Any other material properties
    />
  }
/>
```

Enable shadows using the `castShadow` and `recieveShadow` prop.

> Note: Shadows only work with a custom material. Shadows will not work with `meshBasicMaterial` and `shaderMaterial` by default.

```jsx
<Html
  occlude
  castShadow // Make HTML cast a shadow
  receiveShadow // Make HTML receive shadows
  material={<meshPhysicalMaterial side={DoubleSide} opacity={0.1} />}
/>
```

> Note: Html 'blending' mode only correctly occludes rectangular HTML elements by default. Use the `geometry` prop to swap the backing geometry to a custom one if your Html has a different shape.


#### useFBO

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/misc-usefbo--use-fbo-st)

Creates a `THREE.WebGLRenderTarget`.

```tsx
type FBOSettings = {
  /** Defines the count of MSAA samples. Can only be used with WebGL 2. Default: 0 */
  samples?: number
  /** If set, the scene depth will be rendered into buffer.depthTexture. Default: false */
  depth?: boolean
} & THREE.WebGLRenderTargetOptions

export function useFBO(
  /** Width in pixels, or settings (will render fullscreen by default) */
  width?: number | FBOSettings,
  /** Height in pixels */
  height?: number,
  /**Settings */
  settings?: FBOSettings
): THREE.WebGLRenderTarget {
```

```jsx
const target = useFBO({ stencilBuffer: false })
```

The rendertarget is automatically disposed when unmounted.


```jsx
const { fbo, camera, update } = useCubeCamera()
```

#### useDetectGPU

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/misc-usedetectgpu)

This hook uses [DetectGPU by @TimvanScherpenzeel](https://github.com/TimvanScherpenzeel/detect-gpu), wrapped into suspense, to determine what tier should be assigned to the user's GPU.

👉 This hook CAN be used outside the @react-three/fiber `Canvas`.

```jsx
function App() {
  const GPUTier = useDetectGPU()
  // show a fallback for mobile or lowest tier GPUs
  return (
    {(GPUTier.tier === "0" || GPUTier.isMobile) ? <Fallback /> : <Canvas>...</Canvas>

<Suspense fallback={null}>
  <App />
```

#### useAspect

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/misc-useaspect--default-story)

This hook calculates aspect ratios (for now only what in css would be `image-size: cover` is supported). You can use it to make an image fill the screen. It is responsive and adapts to viewport resize. Just give the hook the image bounds in pixels. It returns an array: `[width, height, 1]`.

```jsx
const scale = useAspect(
  1024,                     // Pixel-width
  512,                      // Pixel-height
  1                         // Optional scaling factor
)
return (
  <mesh scale={scale}>
    <planeGeometry />
    <meshBasicMaterial map={imageTexture} />
```

#### useIntersect

<p>
  <a href="https://codesandbox.io/s/gsm1y"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/gsm1y/screenshot.png" alt="Demo"/></a>
</p>

A very cheap frustum check that gives you a reference you can observe in order to know if the object has entered the view or is outside of it. This relies on [THREE.Object3D.onBeforeRender](https://threejs.org/docs/#api/en/core/Object3D.onBeforeRender) so it only works on objects that are effectively rendered, like meshes, lines, sprites. It won't work on groups, object3d's, bones, etc.

```jsx
const ref = useIntersect((visible) => console.log('object is visible', visible))
return <mesh ref={ref} />
```

# Loading

#### useGLTF

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/loaders-gltf)

A convenience hook that uses `useLoader` and `GLTFLoader`, it defaults to CDN loaded draco binaries (`https://www.gstatic.com/draco/v1/decoders/`) which are only loaded for compressed models.

```jsx
useGLTF(url)

useGLTF(url, '/draco-gltf')

useGLTF.preload(url)
```

If you want to use your own draco decoder globally, you can pass it through `useGLTF.setDecoderPath(path)`:

> **Note** <br>If you are using the CDN loaded draco binaries, you can get a small speedup in loading time by prefetching them.
>
> You can accomplish this by adding two `<link>` tags to your `<head>` tag, as below. The version in those URLs must exactly match what [useGLTF](src/core/useGLTF.tsx#L18) uses for this to work. If you're using create-react-app, `public/index.html` file contains the `<head>` tag.
>
> ```html
> <link
>   rel="prefetch"
>   crossorigin="anonymous"
>   href="https://www.gstatic.com/draco/versioned/decoders/1.5.5/draco_wasm_wrapper.js"
> />
> <link
>   rel="prefetch"
>   crossorigin="anonymous"
>   href="https://www.gstatic.com/draco/versioned/decoders/1.5.5/draco_decoder.wasm"
> />
> ```
>
> It is recommended that you check your browser's network tab to confirm that the correct URLs are being used, and that the files do get loaded from the prefetch cache on subsequent requests.


#### useTexture

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/loaders-texture)

A convenience hook that uses `useLoader` and `TextureLoader`

```jsx
const texture = useTexture(url)
const [texture1, texture2] = useTexture([texture1, texture2])
```

You can also use key: url objects:

```jsx
const props = useTexture({
  metalnessMap: url1,
  map: url2,
})
return <meshStandardMaterial {...props} />
```

#### useCubeTexture

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/loaders-cubetexture)

A convenience hook that uses `useLoader` and `CubeTextureLoader`

```jsx
const envMap = useCubeTexture(['px.png', 'nx.png', 'py.png', 'ny.png', 'pz.png', 'nz.png'], { path: 'cube/' })
```


#### useTrailTexture

<p>
  <a href="https://codesandbox.io/s/fj1qlg"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/fj1qlg/screenshot.png" alt="Demo"/></a>
</p>

This hook returns a `THREE.Texture` with a pointer trail which can be used in shaders to control displacement among other things, and a movement callback `event => void` which reads from `event.uv`.

```tsx
type TrailConfig = {
  /** texture size (default: 256x256) */
  size?: number
  /** Max age (ms) of trail points (default: 750) */
  maxAge?: number
  /** Trail radius (default: 0.3) */
  radius?: number
  /** Canvas trail opacity (default: 0.2) */
  intensity?: number
  /** Add points in between slow pointer events (default: 0) */
  interpolate?: number
  /** Moving average of pointer force (default: 0) */
  smoothing?: number
  /** Minimum pointer force (default: 0.3) */
  minForce?: number
  /** Blend mode (default: 'screen') */
  blend?: CanvasRenderingContext2D['globalCompositeOperation']
  /** Easing (default: easeCircOut) */
  ease?: (t: number) => number
}
```

```jsx
const [texture, onMove] = useTrailTexture(config)
return (
  <mesh onPointerMove={onMove}>
    <meshStandardMaterial displacementMap={texture} />
```

#### useFont

Uses THREE.FontLoader to load a font and returns a `THREE.Font` object. It also accepts a JSON object as a parameter. You can use this to preload or share a font across multiple components.

```jsx
const font = useFont('/fonts/helvetiker_regular.typeface.json')
return <Text3D font={font} />
```

In order to preload you do this:

```jsx
useFont.preload('/fonts/helvetiker_regular.typeface.json')
```

# Performance

#### meshBounds

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/misc-meshbounds--mesh-bounds-st)

A very fast, but often good-enough bounds-only raycast for meshes. You can use this if performance has precedence over pointer precision.

```jsx
<mesh raycast={meshBounds} />
```


# Portals

#### Hud

<p>
  <a href="https://codesandbox.io/s/py4db"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/py4db/screenshot.png" alt="Demo"/></a>
</p>

Renders a heads-up-display (HUD). Each HUD is a scene on top of the previous. That scene is inside a React `createPortal` and is completely isolated, you can have your own cameras in there, environments, etc. The first HUD (`renderpriotity === 1`) will clear the scene and render the default scene, it needs to be the first to execute! Make sure to be explicit about the `renderpriority` of your HUDs.

```tsx
type HudProps = {
  /** Any React node */
  children: React.ReactNode
  /** Render priority, default: 1 */
  renderPriority?: number
}
```

```jsx
{
  /* Renders on top of the default scene with a perspective camera */
}
;<Hud>
  <PerspectiveCamera makeDefault position={[0, 0, 10]} />
  <mesh>
    <ringGeometry />
  </mesh>
</Hud>
{
  /* Renders on top of the previous HUD with an orthographic camera */
}
;<Hud renderPriority={2}>
  <OrthographicCamera makeDefault position={[0, 0, 10]} />
  <mesh>
    <boxGeometry />
  </mesh>
</Hud>
```


# Staging

#### Center

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/staging-center--default-story)

<p>
  <a href="https://codesandbox.io/s/x6obrb"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/x6obrb/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/v8s9ij"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/v8s9ij/screenshot.png" alt="Demo"/></a>
</p>

Calculates a boundary box and centers its children accordingly.

```tsx
export type Props = JSX.IntrinsicElements['group'] & {
  top?: boolean
  right?: boolean
  bottom?: boolean
  left?: boolean
  front?: boolean
  back?: boolean
  /** Disable all axes */
  disable?: boolean
  /** Disable x-axis centering */
  disableX?: boolean
  /** Disable y-axis centering */
  disableY?: boolean
  /** Disable z-axis centering */
  disableZ?: boolean
  /** Precision, defaults to true, see https://threejs.org/docs/index.html?q=box3#api/en/math/Box3.setFromObject */
  precise?: boolean
  /** Callback, fires in the useLayoutEffect phase, after measurement */
  onCentered?: (props: OnCenterCallbackProps) => void
}
```

```tsx
type OnCenterCallbackProps = {
  /** The next parent above <Center> */
  parent: THREE.Object3D
  /** The outmost container group of the <Center> component */
  container: THREE.Object3D
  width: number
  height: number
  depth: number
  boundingBox: THREE.Box3
  boundingSphere: THREE.Sphere
  center: THREE.Vector3
  verticalAlignment: number
  horizontalAlignment: number
  depthAlignment: number
}
```

```jsx
<Center top left>
  <mesh />
</Center>
```

Optionally you can define `onCentered` which calls you back when contents have been measured. This would allow you to easily scale to fit. The following for instance fits a model to screen height.

```jsx
function ScaledModel() {
  const viewport = useThree((state) => state.viewport)
  return (
    <Center onCentered={({ container, height }) => container.scale.setScalar(viewport.height / height)}>
      <Model />
    </Center>
```

#### Resize

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/staging-resize)

<p>
  <a href="https://codesandbox.io/s/6yg0i3"><img width="20%" src="https://user-images.githubusercontent.com/76580/234665568-2be311d2-1896-4f82-ae20-b10b44c1e952.png" alt="Demo"/></a>
</p>

Calculates a boundary box and scales its children so the highest dimension is constrained by 1. NB: proportions are preserved.

```tsx
export type ResizeProps = JSX.IntrinsicElements['group'] & {
  /** constrained by width dimension (x axis), undefined */
  width?: boolean
  /** constrained by height dimension (y axis), undefined */
  height?: boolean
  /** constrained by depth dimension (z axis), undefined */
  depth?: boolean
  /** You can optionally pass the Box3, otherwise will be computed, undefined */
  box3?: THREE.Box3
  /** See https://threejs.org/docs/index.html?q=box3#api/en/math/Box3.setFromObject */
  precise?: boolean
}
```

```jsx
<Resize>
  <mesh />
</Resize>
```

You can also specify the dimension to be constrained by:

```jsx
<Resize height>
  <Box args={[70, 40, 20]}>
</Resize>
```

#### BBAnchor

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.vercel.app/?path=/story/misc-bbanchor--bb-anchor-with-html)

A component using AABB (Axis-aligned bounding boxes) to offset children position by specified multipliers (`anchor` property) on each axis. You can use this component to change children positioning in regard of the parent's bounding box, eg. pinning [Html](#html) component to one of the parent's corners. Multipliers determine the offset value based on the `AABB`'s size:

```
childrenAnchor = boundingBoxPosition + (boundingBoxSize * anchor / 2)
```

```jsx
<BBAnchor
  anchor // THREE.Vector3 or [number, number, number]
  {...groupProps} // All THREE.Group props are valid
>
  {children}
</BBAnchor>
```

For instance, one could want the Html component to be pinned to `positive x`, `positive y`, and `positive z` corner of a [Box](#shapes) object:

```jsx
<Box>
  <BBAnchor anchor={[1, 1, 1]}>
    <Html center>
      <span>Hello world!</span>
    </Html>
  </BBAnchor>
</Box>
```

#### Bounds

<p>
  <a href="https://codesandbox.io/s/rz2g0"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/rz2g0/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/42glz0"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/42glz0/screenshot.png" alt="Demo"/></a>
</p>

Calculates a boundary box and centers the camera accordingly. If you are using camera controls, make sure to pass them the `makeDefault` prop. `fit` fits the current view on first render. `clip` sets the cameras near/far planes. `observe` will trigger on window resize.

```jsx
<Bounds fit clip observe damping={6} margin={1.2}>
  <mesh />
</Bounds>
```

The Bounds component also acts as a context provider, use the `useBounds` hook to refresh the bounds, fit the camera, clip near/far planes, go to camera orientations or focus objects. `refresh(object?: THREE.Object3D | THREE.Box3)` will recalculate bounds, since this can be expensive only call it when you know the view has changed. `clip` sets the cameras near/far planes. `to` sets a position and target for the camera. `fit` zooms and centers the view.

```jsx
function Foo() {
  const bounds = useBounds()
  useEffect(() => {
    // Calculate scene bounds
    bounds.refresh().clip().fit()

    // Or, focus a specific object or box3
    // bounds.refresh(ref.current).clip().fit()
    // bounds.refresh(new THREE.Box3()).clip().fit()

    // Or, send the camera to a specific orientatin
    // bounds.to({position: [0, 10, 10], target: {[5, 5, 0]}})
<Bounds>
  <Foo />
```


#### Environment

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/staging-environment--environment-story)

<p>
  <a href="https://codesandbox.io/s/t4l0f"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/t4l0f/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/mih0lx"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/mih0lx/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/e662p3"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/e662p3/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/lwo219"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/lwo219/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/q48jgy"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/q48jgy/screenshot.png" alt="Demo"/></a>
  <a href="https://codesandbox.io/s/0c5hv9"><img width="20%" src="https://codesandbox.io/api/v1/sandboxes/0c5hv9/screenshot.png" alt="Demo"/></a>
</p>

Sets up a global cubemap, which affects the default `scene.environment`, and optionally `scene.background`, unless a custom scene has been passed. A selection of [presets](src/helpers/environment-assets.ts) from [HDRI Haven](https://hdrihaven.com/) are available for convenience. If you pass an array of files it will use THREE.CubeTextureLoader.

```jsx
<Environment
  background={false} // can be true, false or "only" (which only sets the background) (default: false)
  blur={0} // blur factor between 0 and 1 (default: 0, only works with three 0.146 and up)
  files={['px.png', 'nx.png', 'py.png', 'ny.png', 'pz.png', 'nz.png']}
  path="/"
  preset={null}
  scene={undefined} // adds the ability to pass a custom THREE.Scene, can also be a ref
  encoding={undefined} // adds the ability to pass a custom THREE.TextureEncoding (default: THREE.sRGBEncoding for an array of files and THREE.LinearEncoding for a single texture)
/>
```

The simplest way to use it is to provide a preset. 👉 Note: `preset` property is not meant to be used in production environments and may fail as it relies on CDNs.

```jsx
<Environment preset="city" />
```

If you provide a single string it will use THREE.RGBELoader.

```jsx
<Environment files="file.hdr" />
```

You can also use [@pmndrs/assets](https://github.com/pmndrs/assets) to easily self host common assets. Always use dynamic imports to avoid making this part of your main bundle.

```jsx
import { suspend } from 'suspend-react'
const city = import('@pmndrs/assets/hdri/city.exr').then((module) => module.default)

<Environment files={suspend(city)} />
```

If you already have a cube texture you can pass it directly:

```jsx
<CubeCamera>{(texture) => <Environment map={texture} />}</CubeCamera>
```

If you provide children you can even render a custom environment. It will render the contents into an off-buffer and film a single frame with a cube camera (whose props you can configure: near=1, far=1000, resolution=256).

```jsx
<Environment background near={1} far={1000} resolution={256}>
  <mesh scale={100}>
    <sphereGeometry args={[1, 64, 64]} />
    <meshBasicMaterial map={texture} side={THREE.BackSide} />
  </mesh>
</Environment>
```

You can even mix a generic HDRI environment into a custom one with either the `preset` or the `files` prop.

```jsx
return (
  <Environment background near={1} far={1000} resolution={256} preset="warehouse">
    <mesh />
```

Declarative environment content can also animate with the `frames` prop, the envmap can be live. Give it a low resolution and this will happen at very little cost

```jsx
return (
  <Environment frames={Infinity} resolution={256}>
    <Float>
      <mesh />
    </Float>
```

Environment can also be ground projected, that is, put your model on the "ground" within the environment map.

```jsx
<Environment ground />
```

You can provide optional options to configure this projecion.

```jsx
<Environment
  ground={{
    height: 15, // Height of the camera that was used to create the env map (Default: 15)
    radius: 60, // Radius of the world. (Default 60)
    scale: 1000, // Scale of the backside projected sphere that holds the env texture (Default: 1000)
  }}
/>
```

#### useEnvironment

A convenience hook to load an environment map. The props are the same as on the `<Environment />` component.

```tsx
export type EnvironmentLoaderProps = {
  files?: string | string[]
  path?: string
  preset?: PresetsType
  extensions?: (loader: Loader) => void
  encoding?: TextureEncoding
```

You can use it without properties, which will default to px, nx, py, ny, pz, nz as \*.png files inside your /public directory.

```jsx
const cubeTexture = useEnvironment()
```

Or you can specificy from where to load the files.

```jsx
const presetTexture = useEnvironment({ preset: 'city' })
const rgbeTexture = useEnvironment({ files: 'model.hdr' })
const cubeTexture = useEnvironment({ files: ['px', 'nx', 'py', 'ny', 'pz', 'nz'].map((n) => `${n}.png`) })
```

#### useMatcapTexture

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/staging-usematcaptexture--use-matcap-texture-st) ![](https://img.shields.io/badge/-suspense-brightgreen)

Loads matcap textures from this repository: https://github.com/emmelleppi/matcaps

(It is a fork of this repository: https://github.com/nidorx/matcaps)

👉 Note: `useMatcapTexture` hook is not meant to be used in production environments as it relies on third-party CDN.

```jsx
const [matcap, url] = useMatcapTexture(
 0, // index of the matcap texture https://github.com/emmelleppi/matcaps/blob/master/matcap-list.json
 1024 // size of the texture ( 64, 128, 256, 512, 1024 )
)

return (
 ...
 <meshMatcapMaterial matcap={matcap} />
 ...
)
```

👉 You can also use the exact name of the matcap texture, like so:

```jsx
const [matcap] = useMatcapTexture('3E2335_D36A1B_8E4A2E_2842A5')
```

👉 Use the `url` to download the texture when you are ready for production!

#### useNormalTexture

[![](https://img.shields.io/badge/-storybook-%23ff69b4)](https://drei.pmnd.rs/?path=/story/staging-usenormaltexture--use-normal-texture-st) ![](https://img.shields.io/badge/-suspense-brightgreen)

Loads normal textures from this repository: https://github.com/emmelleppi/normal-maps

👉 Note: `useNormalTexture` hook is not meant to be used in production environments as it relies on third-party CDN.

```jsx
const [normalMap, url] = useNormalTexture(
  1, // index of the normal texture - https://github.com/emmelleppi/normal-maps/blob/master/normals.json
  // second argument is texture attributes
  {
    offset: [0, 0],
    repeat: [normRepeat, normRepeat],
    anisotropy: 8
  }
)

return (
  ...
  <meshStandardMaterial normalMap={normalMap} />
  ...
)
```
