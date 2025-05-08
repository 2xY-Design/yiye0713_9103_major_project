# Week9 Quiz

## Imaging Technique Inspiration

Inspired by ‘Circles in the Sand’ by Simon’s mandalas (see images below), I plan to replicate the equally spaced dots layered in rings around a central axis. This radial pattern fosters harmony and hierarchical complexity, guiding viewers’ eyes outward in balanced measures. For the major assignment, using parametrically generated rings will provide precise control over dot count, radius steps, and color transitions, ensuring a reproducible, mathematically grounded design that meets requirements for symmetry, scalability, and algorithmic generation within the project timeline.

![An image of 'circles in the sand'](https://growingwell.b-cdn.net/wp-content/uploads/2024/08/Beach-Mandala-Growing-Well-1.webp)

![An image of 'circles in the sand'](https://growingwell.b-cdn.net/wp-content/uploads/2024/08/Beach-Mandala-Growing-Well-2.webp)

## Coding Technique Exploration

The artwork my team picked is the “Wheels of Fortune”. I may use the p5.Polar library for p5.js to abstract all the polar-to-Cartesian math to draw perfect concentric dot-rings without manual sine/cosine loops, tweak ring count, spacing, and styling in one place:

```
setCenter(width/2, height/2);
polarGrid(rings, steps, rStep, angleOffset, (r, θ) => {
  point(r, θ);
});
```

[A Code Example from Openprocessing](https://openprocessing.org/sketch/1879782)