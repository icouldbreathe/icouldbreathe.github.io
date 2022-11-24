---
title: "Learning project: Ray Tracer"
description: "A personal learning project to learn and implement ray tracing in C++."
current: true
repository: https://github.com/icouldbreathe/Raytracer
technology: C++
---
<img align="right" src="/assets/img/ray-tracer/rtiow-final-render.png" alt="RTIOW Final Render" style="margin: 0 10px 10px 10px;width:20em;" />
I have picked up this project to learn more about graphics programming, particularly offline rendering. In this case it is a ray tracer or more technically a path tracer. In essence it is an algorithm that calculates a pixel value based on ray-object interaction. Given different material types and their properties, different behaviour can be expected once the ray hits the object, simulating real-life physics of light scattering, reflection and refraction. The end result ends up producing photo-realistic images.

While this is a fairly general and simple solution, it was a good introduction to graphics programming and rendering. I have to thank the online book series [Ray Tracing in One Weekend by Peter Shirley](https://raytracing.github.io/) for providing an easy to follow and concise introduction to ray tracing.

### Progress

-   Output an image (PPM)
-   Implement progress indicator
-   Implement basic vector class
-   Implement basic ray class
-   Implement basic camera, viewport and background
-   Implement a build solution (make)
-   Ray-Sphere intersection
-   Surface normals and multiple objects
-   Antialiasing
-   Diffuse materials
-   Metal
-   Dielectrics
-   Positionable Camera
-   Defocus Blur
-   Final Render
-   Multithreading

### Going forward

As of now I have finished the first book of the series and would love to improve on it. Several ideas come to mind:

* ~~Make it render faster. It can take a while to render a simple scene. One way to make it faster would be to introduce multithreading.~~
* Implement more type of primitives for the rays to interact with.
* Add proper mesh I/O system, so that I could import more interesting models.
* Implement live rendering. Right now the method to render an image is very primitive and using a graphics API to display the results live would be a cool feature.

### Updates

**24-11-2022 •**
I have implemented some multithreading to speed up the rendering process. I have divided portions of the image to be rendered based on how many hardware concurrent threads are available. Without multithreading, a 200x133 pixel image takes about 21 seconds to render. With multithreading, using 4 threads, it takes around 12 seconds to render, which is an improvement of ~42% in speed.
