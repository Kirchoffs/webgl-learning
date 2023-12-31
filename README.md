# Notes

## Cavas API
- 2D
- CanvasRenderingContext2D
- canvas.getContext('2d')

### Canvas Coordinate System
The origin of the canvas coordinate space is the top-left corner of the canvas element. The x-axis is horizontal and positive to the right, and the y-axis is vertical and positive downwards.

## WebGL API
__WebGL__ is based on __OpenGL ES 2.0__, and __WebGL 2__ is based on __OpenGL ES 3.0__.

- 3D
- WebGLRenderingContext
- canvas.getContext('webgl')
- WebGL2RenderingContext
- canvas.getContext('webgl2')

### WebGL Coordinate System
The origin of the WebGL coordinate space is the center of the canvas element. The x-axis is horizontal and positive to the right, and the y-axis is vertical and positive upwards.

### Right Handed Coordinate System
The WebGL coordinate system is a __right handed__ coordinate system. This means that the positive z-axis comes out of the screen towards the viewer.

For right handed coordinate system, thumb points to x-axis, index finger points to y-axis, and middle finger points to z-axis.

In physics, the right hand coordinate system is commonly used.

## Rendering
There are three main distinctions to make when discussing rendering: software-based and hardware-based rendering, server-based and client-based rendering, and retained-mode and immediate-mode rendering. WebGL offers a unique approach to hardware and client based rendering with an immediate-mode API on the web.

## WebGL Details
```
gl.clear(gl.COLOR_BUFFER_BIT);
gl.clearColor(0.0, 0.0, 0.0, 1.0);

gl.clear(gl.DEPTH_BUFFER_BIT);
gl.clearDepth(1.0);

gl.clear(gl.STENCIL_BUFFER_BIT);
gl.clearStencil(0);
```
