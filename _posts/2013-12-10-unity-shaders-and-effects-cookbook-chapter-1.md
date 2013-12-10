---
layout: post
title: "Unity Shaders and Effects Cookbook: Chapter 1"
categories:
- 
tags:
- 


---
## Diffuse Shading

这章主要讲：
- Creating a basic *Surface Shader*
- Adding properties to a Surface Shader
- Using properties in a Surface Shader
- Create a custom diffuse lighting model
- Create a Half Lambert lighting model
- Create a ramp texture to control diffuse shading
- Creating a faked BRDF using a 2D ramp texture

好的Shader大多开始于基础的diffuse component或者lighting model,在早期的computer graphics,diffuse shading是通过固定光照模型实现的*fixed function lighting model* 它只提供给图形程序单一的光照模型，通过一组参数parameters和贴图textures进行微调。在当前的工业应用中，我们可以使用Cg控制更多，或者在Unity中使用Surface Shaders.

The diffuse component of a Shader basically describes the way *light reflects off a surface in all directions*. 这可能跟如何描述镜面反射(reflective mirror)很像。但它们并不相同。diffuse lighting takes all the light from light source, such as the sun, and reflects its light back to the viewer's eye.


