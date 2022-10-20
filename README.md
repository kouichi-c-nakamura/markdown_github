# markdown_github

mathjax trials


# Positive control

When $a \ne 0$, there are two solutions to $(ax^2 + bx + c = 0)$ and they are

$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$

`\eqalign{..}` can work with `\\`

$$
\eqalign{\sin(90˚ - \theta) &= \cos\theta \\
\cos(90˚ - \theta) &= \sin\theta \\
\tan(90˚ - \theta) &= \frac{1}{\tan\theta} \\
}
$$


`\\` is recognized in `\eqalign{..}`

$$
\eqalign{
\sin \theta &= \tan \theta \cdot \cos \theta \\
\tan ^2 \theta \cdot \cos^2 \theta + \cos ^2 \theta &= 1 \\
1 + \tan ^2 \theta &= \frac {1} {\cos^2 \theta} }
$$

# Broken

`\\` is not recognized 

$$
\sin \theta = \tan \theta \cdot \cos \theta \\
\tan ^2 \theta \cdot \cos^2 \theta + \cos ^2 \theta = 1 \\
1 + \tan ^2 \theta = \frac {1} {\cos^2 \theta}
$$


`\\` is not recognized in `\color {gray} {....}`

$$
\color{gray}{\sin \theta = \tan \theta \cdot \cos \theta より} \\
\color{gray}{\tan^2 \theta \cdot \cos^2 \theta + \cos ^2\theta = 1} \\
1 + \tan ^2 \theta = \frac{1}{\cos^2 \theta}
$$

No blank line  before `$$`
$$
\color{gray}{\sin \theta = \tan \theta \cdot \cos \theta より} \\
\color{gray}{\tan^2 \theta \cdot \cos^2 \theta + \cos ^2\theta = 1} \\
1 + \tan ^2 \theta = \frac{1}{\cos^2 \theta}
$$

Blank line between `$$` and the content

$$

\eqalign{\sin(90˚ - \theta) &= \cos\theta \\
\cos(90˚ - \theta) &= \sin\theta \\
\tan(90˚ - \theta) &= \frac{1}{\tan\theta} \\
}
$$

$$
\eqalign{\sin(90˚ - \theta) &= \cos\theta \\
\cos(90˚ - \theta) &= \sin\theta \\
\tan(90˚ - \theta) &= \frac{1}{\tan\theta} \\
}

$$
