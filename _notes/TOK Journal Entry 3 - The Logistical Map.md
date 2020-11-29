---
title: TOK Journal Entry 3 - The Logistical Map
mathjax: true
---

My third real-life situation is from a [video by Veritasium](https://youtu.be/ovJcsL7vyrk) which talks about how the equation below connects a leaky tap, a population of rabbits and the Mandelbrot set.

$$ \begin{equation*} 	x_{n+1} = rx_{n} \times \left(1-x_{n}\right) \end{equation*} $$

![Mandelbrot set](https://upload.wikimedia.org/wikipedia/commons/2/21/Mandel_zoom_00_mandelbrot_set.jpg)
_The Mandelbrot set_

This real-life situation clearly links to the mathematical area of knowledge as it is an equation that is able to model multiple aspects of our world. Before I explain why this equation is so interesting, we have to understand what this equation does.

Using the example of a rabbit population, the part $x_{n+1}$ refers to the change in population size as a percentage of the original, $x_{n}$, and $r$ is the growth rate. However, this equation would show that the population of rabbits skyrockets to infinity. To stop this, we have to use limiter $(1-x_{n})$ which multiplies $rx_{n}$ by a decimal to slow down its growth.

To more recursions you take of the equation, the more you'll see it stabilise at a particular value regardless of the initial population. Since the initial population doesn't matter, the growth rate $r$ is where this gets interesting. In the lower values of $r$ the population will always go extinct but once $r = 1$, the population stabilises at a positive value. But once $r = 3$, the population begins to jump between two separate points. If you were to graph $r$ against $x_{n+1}$, you'd get this:

![Logistic map](https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Logistic_Bifurcation_map_High_Resolution.png/1200px-Logistic_Bifurcation_map_High_Resolution.png)

This means that the population stabilises not at _one single point, but two_. This splits up once again into four different points and continues to double. Once $r = 3.57$, there's no stable population and chaos emerges. This is a useful property and was first used to generate (pseudo) randomness from computers.

Going back to the Mandelbrot set I mentioned, the way these two relate is that the logistic map _is part of the Mandelbrot set_. To see this, we have to view the set using the z-axis which gives us this image:

![Mandelbrot set with logistic map](https://notes.manassadasivuni.com/assets/img/tok%203/Mandelbrot%20set%20with%20logistic%20map.png)

These unexpected relations have led me to the knowledge question, "To what extent do mathematical equations describe our world?" I feel that this question has no clear answer as it can be argued that math was invented than discovered. From this viewpoint, math doesn't describe our world accurately as it was not part of this world in the first place and we merely use it to attempt to form some relation that we can then break down and analyse.

At the same time, math is widely used in all professions and is used extensively to create models or create products. Due to this, we have the potential ability to describe everything using a combination of numbers and algebra and could argue that math describes everything around us.

These two polar opposite arguments mean that your answer to this question is highly variable upon your view of the origin of mathematics. I personally feel that math is a useful tool to interpret our surroundings, but also that it shouldn't be used to describe everything as there are aspects like emotions that cannot be quantified and attempting to do so would create a flawed model and would be counterintuitive.