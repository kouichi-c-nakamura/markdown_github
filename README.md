# Mathjax behaviour on GitHub

GitHub supports rendering Mathjax. However, its implelementation appears to be very strict and often fails when other renderers are fine.

Here are some examples of successful and unsuccessful usage of Mathjax in GitHub markdown.

# Success

When $a \ne 0$, there are two solutions to $(ax^2 + bx + c = 0)$ and they are

$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$

## `\eqalign{..}` can work with `\\`

$$
\eqalign{\sin(90˚ - \theta) &= \cos\theta \\
\cos(90˚ - \theta) &= \sin\theta \\
\tan(90˚ - \theta) &= \frac{1}{\tan\theta} \\
}
$$

Another example

$$
\eqalign{
\sin \theta &= \tan \theta \cdot \cos \theta \\
\tan ^2 \theta \cdot \cos^2 \theta + \cos ^2 \theta &= 1 \\
1 + \tan ^2 \theta &= \frac {1} {\cos^2 \theta} }
$$

# Broken

## a space between $ and the content 

```
When $ a \ne 0$, there are two solutions to $(ax^2 + bx + c = 0) $ and they are
```

When $ a \ne 0$, there are two solutions to $(ax^2 + bx + c = 0) $ and they are

## no space between $ and the surrounding

```
When$a \ne 0$, there are two solutions to $(ax^2 + bx + c = 0) $and they are
```

When$a \ne 0$, there are two solutions to $(ax^2 + bx + c = 0) $and they are


## `\\` is not recognized for virtually no reason


```
$$
f=\\
1 \\
$$
```

$$
f=\\
1 \\
$$

```
$$
\sin \theta =\\
1 \\
$$
```

$$
\sin \theta =\\
1 \\
$$

```
$$
\sin \theta = \tan \theta \cdot \cos \theta \\
\tan ^2 \theta \cdot \cos^2 \theta + \cos ^2 \theta = 1 \\
1 + \tan ^2 \theta = \frac {1} {\cos^2 \theta}
$$
```

$$
\sin \theta = \tan \theta \cdot \cos \theta \\
\tan ^2 \theta \cdot \cos^2 \theta + \cos ^2 \theta = 1 \\
1 + \tan ^2 \theta = \frac {1} {\cos^2 \theta}
$$

## `\\` is not recognized in `\color {gray} {....}`

```
$$
\color{gray}{\sin \theta = \tan \theta \cdot \cos \theta より} \\
\color{gray}{\tan^2 \theta \cdot \cos^2 \theta + \cos ^2\theta = 1} \\
1 + \tan ^2 \theta = \frac{1}{\cos^2 \theta}
$$
```

$$
\color{gray}{\sin \theta = \tan \theta \cdot \cos \theta より} \\
\color{gray}{\tan^2 \theta \cdot \cos^2 \theta + \cos ^2\theta = 1} \\
1 + \tan ^2 \theta = \frac{1}{\cos^2 \theta}
$$

## No blank line above `$$`

```
abcde
$$
\color{gray}{\sin \theta = \tan \theta \cdot \cos \theta より} \\
\color{gray}{\tan^2 \theta \cdot \cos^2 \theta + \cos ^2\theta = 1} \\
1 + \tan ^2 \theta = \frac{1}{\cos^2 \theta}
$$
```

abcde
$$
\color{gray}{\sin \theta = \tan \theta \cdot \cos \theta より} \\
\color{gray}{\tan^2 \theta \cdot \cos^2 \theta + \cos ^2\theta = 1} \\
1 + \tan ^2 \theta = \frac{1}{\cos^2 \theta}
$$

## Existence of a blank line between `$$` and the content

```
$$

\eqalign{\sin(90˚ - \theta) &= \cos\theta \\
\cos(90˚ - \theta) &= \sin\theta \\
\tan(90˚ - \theta) &= \frac{1}{\tan\theta} \\
}
$$
```

$$

\eqalign{\sin(90˚ - \theta) &= \cos\theta \\
\cos(90˚ - \theta) &= \sin\theta \\
\tan(90˚ - \theta) &= \frac{1}{\tan\theta} \\
}
$$

```
$$
\eqalign{\sin(90˚ - \theta) &= \cos\theta \\
\cos(90˚ - \theta) &= \sin\theta \\
\tan(90˚ - \theta) &= \frac{1}{\tan\theta} \\
}

$$
```

$$
\eqalign{\sin(90˚ - \theta) &= \cos\theta \\
\cos(90˚ - \theta) &= \sin\theta \\
\tan(90˚ - \theta) &= \frac{1}{\tan\theta} \\
}

$$
