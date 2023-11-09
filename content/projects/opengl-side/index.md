---
title: OpenGL w/ GLFW and ImGUI Engine Prototype
seo_title: OpenGL w/ GLFW and ImGUI Engine Prototype
summary: Learning OpenGL and the graphics pipeline to display pixels and objects on the screen.
description: 
slug: opengl-side
author: Dovydas Ciomenas

draft: false
date: 2018
lastmod: 
expiryDate: 
publishDate: 

feature_image: 2d.png
feature_image_alt: 

project types: [Prototype, Learning]

techstack: [C++, OpenGL, GLFW, GLM, GLSL, GLAD, ImGUI]
live_url: 
source_url: https://github.com/icouldbreathe/sideproj-learn-opengl

newsletter: false
---

While this is purely a learning project and is definitely not finished, I am including this here to document my progress and provide the source code.

I picked up this project to learn graphics programming, particularly OpenGL, its graphics pipeline, vertex and index buffers, textures, vertex and fragment shaders w/ GLSL, as well as the 3D maths required for camera setup, transforms, translations and lighting. The solution uses GLAD as the OpenGL extension loader, GLFW for window management, GLM as the maths library, ImGUI for GUI and displaying information.

The application has three tests: solid color, 2D textures and a 3D model.

<small>Select color test.</small>
![Color](color.png)

<small>Display 2D textures and translate test.</small>
![2D](2d.png)

<small>Display 3D object.</small>
![3D](3d.png)
