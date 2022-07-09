---
title: "Personal project: Ray Tracer"
description: "A personal learning project to learn and implement ray tracing in C++."
current: true
repository: https://github.com/icouldbreathe/Raytracer
technology: C++
---

Graphics programming is one of my interests and this project is meant to deepen my knowledge in this field, particularly with ray tracing and how it works. I have found that the online book series [Ray Tracing in One Weekend by Peter Shirley](https://raytracing.github.io/) is a good place to start and offers an easy to read, step-by-step explanation and covers both the programming side and the maths behind it.

## My current progress with the project:

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

## Final Render

I have made the final render of a scene including materials of diffuse, metal and dielectric type:

<img src="/assets/img/ray-tracer/rtiow-final-render.png" alt="RTIOW Final Render" style="margin-bottom: 0px;" />
<small>Final Render</small>

## Going forward

As of now I have finished the first book of the series and plan to improve on it. Several ideas come to mind:

* Make it render faster. It can take a while to render a simple scene. One way to make it faster would be to introduce multithreading.
* Implement more type of primitives for the rays to interact with.
* Add proper mesh I/O system, so that I could import more interesting models.
* Implement live rendering. Right now the method to render an image is very primitive and using a graphics API to display the results live would be a cool feature.

You can see the current progress on my GitHub page.
