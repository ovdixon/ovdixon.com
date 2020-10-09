---
title: "Generative Art 🖼"
date: 2019-03-09T19:22:42+11:00
draft: false
summary: "An exploration into computer generated art."
---

Computational systems allow for the realization and expression of ideas that are impossible in other media, or in reality. In such a way, generative computer art is a medium of expression beyond the realm of conventional art, one in which difference can be created within indifference. As part of a university course I took in Design Programming I was required to submit a design inspired by an historical example of computer art.


#### Inspiration
Georg Nees was a German academic who is considered one of the pioneers of computer art and generative graphics. He was interested in the relationship between order and disorder in picture composition. This is reflected in the untitled artwork below; Here Nees has introduced random variables into the computer program to produce the disordered lines. These lines are framed within the ordered circles to produce a striking contrast. This artwork served as the inspiration for my own exploration into the practice of generative computer art.

{{< figure src="untitled.png" caption="Untitled artwork by Georg Nees">}}


#### Implementation

My design was created using [p5.js](https://p5js.org). This is a client-side library for creating graphic and interactive experiences, based on the core principles of Processing. You can view view the code and live design [here](https://www.openprocessing.org/sketch/687721) (doesn't work well in Safari).

{{< figure src="generations.png" caption="Six random generations of my design">}}

 I sought to create a program which would produce ordered patterns from the intersection of two seemingly disordered sets of lines. The absence of any border around the pattern is designed to evoke a sense of curiosity towards the direction and origin of the lines. The experience of being drawn into the pattern before the program generates a new pattern, is a provocative source of thought for the viewer about whether machines can produce works of artistic value.