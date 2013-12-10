---
layout: post
title: "Unity Shaders and Effects Cookbook: Chapter 1"
categories:
- 
tags:
- 


---
## Diffuse Shading

������Ҫ����
- Creating a basic *Surface Shader*
- Adding properties to a Surface Shader
- Using properties in a Surface Shader
- Create a custom diffuse lighting model
- Create a Half Lambert lighting model
- Create a ramp texture to control diffuse shading
- Creating a faked BRDF using a 2D ramp texture

�õ�Shader��࿪ʼ�ڻ�����diffuse component����lighting model,�����ڵ�computer graphics,diffuse shading��ͨ���̶�����ģ��ʵ�ֵ�*fixed function lighting model* ��ֻ�ṩ��ͼ�γ���һ�Ĺ���ģ�ͣ�ͨ��һ�����parameters����ͼtextures����΢�����ڵ�ǰ�Ĺ�ҵӦ���У����ǿ���ʹ��Cg���Ƹ��࣬������Unity��ʹ��Surface Shaders.

The diffuse component of a Shader basically describes the way *light reflects off a surface in all directions*. ����ܸ�����������淴��(reflective mirror)���񡣵����ǲ�����ͬ��diffuse lighting takes all the light from light source, such as the sun, and reflects its light back to the viewer's eye.


