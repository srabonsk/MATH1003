# Module 1 Study Guide: Functions and Graphs

Oct 8, 2026 · @Shaikh Srabon

This guide covers every Module 1 outcome in plain steps, with the traps that cost you marks in Assignments 1 to 5.

## Start here

If you only have two hours tonight, do sections 2, 5, 6 and 9 first, then take the practice test in section 10.

| Priority | Section | Why it matters |
| --- | --- | --- |
| 1 | Domain, range, intervals | Shows up in every topic, and limits depend on it |
| 2 | Transformations and composition | Quick points once you know the table |
| 3 | Inverses | One 3-step method, easy to drill |
| 4 | Exp and log equations | Same few moves every time |
| 5 | Trig and inverse trig | Memorize the unit circle once |

How to use each section: read the rule, cover the worked example, solve it yourself, then check. Reading alone will not stick.

## Domain, range and interval notation

The domain is every x you are allowed to plug in. The range is every y that comes out.

**Three things break a function.** Check the formula for each:

1. An even root (square root, 4th root) of a negative number. Set the inside ≥ 0.
2. A denominator equal to zero. Set the denominator ≠ 0.
3. A log of zero or a negative number. Set the inside > 0.

**Interval notation.** Write the smaller number first. A square bracket includes the endpoint, a parenthesis does not, and infinity always gets a parenthesis.

| In words | Interval |
| --- | --- |
| x > 3 | (3, ∞) |
| x ≥ 3 | \[3, ∞) |
| x ≤ 5 | (−∞, 5\] |
| −2 < x ≤ 6 | (−2, 6\] |
| every x except 5 | (−∞, 5) ∪ (5, ∞) |

**When does the inequality sign flip?** Only when you multiply or divide both sides by a negative number.

```latex
-2x + 6 \ge 0 \;\Rightarrow\; -2x \ge -6 \;\Rightarrow\; x \le 3
```

**Worked example 1.** Domain of the function below.

```latex
f(x) = \frac{\sqrt{7+4x}}{x^2-4}
```

The root needs 7 + 4x ≥ 0, so 4x ≥ −7 and x ≥ −7/4. The denominator needs x ≠ 2 and x ≠ −2. Since −2 is already below −7/4, only x = 2 leaves a gap. Domain: \[−7/4, 2) ∪ (2, ∞). Trap: divide −7 by 4 to get −7/4, not −4/7.

**Worked example 2.** A fraction inside a fraction has two things to check.

```latex
f(x) = \frac{2}{\frac{3}{x} + 5}
```

The inner fraction needs x ≠ 0. The big denominator needs 3/x + 5 ≠ 0, so 3/x ≠ −5, so 3 ≠ −5x, so x ≠ −3/5. Domain: (−∞, −3/5) ∪ (−3/5, 0) ∪ (0, ∞).

**Worked example 3.** ln(9 − x²) needs 9 − x² > 0, so x² < 9, so −3 < x < 3. Domain: (−3, 3).

**Range.** There is no formula check. Picture the graph, find the lowest and highest outputs, and ask whether each one is actually reached (bracket) or only approached (parenthesis).

| Function | Range | Reason |
| --- | --- | --- |
| x² | \[0, ∞) | Lowest point is (0, 0), then it climbs forever |
| −x² + 3 | (−∞, 3\] | Frown shape, highest point is 3 |
| √x | \[0, ∞) | Smallest output is √0 = 0 |
| 1/x | all y except 0 | Gets close to 0 but never reaches it |

## Reading graphs: function test, piecewise, even and odd

**Vertical line test.** A graph is a function of x only if every vertical line crosses it at most once. One x can only have one y.

- Fails: sideways parabolas, circles and ovals, and a stray dot sitting above or below the curve at an x the curve already covers.
- Passes: zigzags, waves, jumps and holes. Wiggly is fine as long as the curve never doubles back over the same x.
- Open circle = that point is not on the graph. Filled dot = it is.

**Piecewise functions.** Different formula on different x-ranges. Pick the piece by checking which range your x falls in.

```latex
f(x) = \begin{cases} 3 & x \le 0 \\ x+3 & 0 < x < 2 \\ 4 & x \ge 2 \end{cases}
```

f(−1) = 3. f(1) = 1 + 3 = 4. f(2) = 4, even though the middle piece was heading toward 5. That gap is a jump. Absolute value is the classic piecewise function: |x| = x when x ≥ 0, and |x| = −x when x < 0.

**Even and odd.** Plug in −x and simplify.

| Type | Test | Symmetry | Examples |
| --- | --- | --- | --- |
| Even | f(−x) = f(x) | mirror across the y-axis | x², cos x, abs(x) |
| Odd | f(−x) = −f(x) | spins onto itself around the origin | x³, sin x, tan x |

Shortcuts:

- Polynomial with only even powers (a constant counts as even): even. Only odd powers: odd. A mix: neither.
- even × even = even. odd × odd = even. even × odd = odd.

**Worked examples.**

| Function | Verdict | Why |
| --- | --- | --- |
| x⁻⁶ | even | even power |
| x² + 3x⁴ + 2x⁵ | neither | mixes even and odd powers |
| −5x² − 3x⁴ − 2 | even | only even powers and a constant |
| x cos x | odd | odd × even |
| cos(2x) / x | odd | even ÷ odd |
| csc(x²) | even | the inside, x², is already even |
| sec²t − 1 | even | it equals tan²t, an odd function squared |

## Function families

**Linear: y = mx + b.** The slope m is rise over run, and b is where the line crosses the y-axis.

```latex
m = \frac{y_2 - y_1}{x_2 - x_1}
```

A line through (0, 6) and (1, 3) has slope (3 − 6)/(1 − 0) = −3 and y-intercept 6. A line through (0, 1) and (3, 2) has slope 1/3 and y-intercept 1.

**Power functions: x to a fixed power.** x² is a U, x³ is an S-curve through the origin, 1/x is a two-branch hyperbola, √x is half of a sideways U.

**Quadratics: ax² + bx + c.**

| Want | How |
| --- | --- |
| Opens up or down | a > 0 is a smile with a minimum. a < 0 is a frown with a maximum |
| Axis of symmetry | x = −b / (2a) |
| Vertex | x = −b / (2a), then plug that x back in to get y |
| y-intercept | the point (0, c) |
| x-intercepts (roots) | quadratic formula, or factor |

```latex
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
```

**Worked example.** f(x) = −5x² − 40x − 58. Vertex x = −(−40) / (2 · −5) = −4. Then f(−4) = −80 + 160 − 58 = 22. So the vertex is (−4, 22), and since a < 0 it is a maximum of 22. For the roots, multiply by −1 to get 5x² + 40x + 58 = 0. The discriminant is 1600 − 1160 = 440, so x = (−40 ± √440) / 10 = −4 ± √110 / 5. That is about −6.098 and −1.902, symmetric around x = −4.

**Worked example.** y = −0.1x² + 0.2x + 2. Opens down. Axis x = −0.2 / (2 · −0.1) = 1. Vertex (1, 2.1). y-intercept (0, 2). Roots: multiply by −10 to get x² − 2x − 20 = 0, so x = 1 ± √21, about 5.58 and −3.58.

**Polynomials.** The degree is the highest power. The domain is always all reals.

**End behavior** depends on the leading term (highest power, with its coefficient):

| Degree | Leading coefficient | Left end | Right end |
| --- | --- | --- | --- |
| even | positive | up | up |
| even | negative | down | down |
| odd | positive | down | up |
| odd | negative | up | down |

Worked example: f(x) = 14(x − 6)¹⁵(4 − x)¹¹. Rewrite (4 − x)¹¹ as −(x − 4)¹¹. The leading term is 14 · x¹⁵ · (−x¹¹) = −14x²⁶. Degree 26 is even and the coefficient is negative, so both ends go down.

**Touch or cross at a root.** A factor to an odd power (like x − 4) crosses the x-axis. A factor to an even power (like (x + 1)²) touches the axis and turns back. So (x + 1)²(x − 4) bounces at x = −1 and crosses at x = 4.

**Rational functions: p(x) / q(x).** The domain is all x where q(x) ≠ 0. A vertical asymptote sits at each zero of the denominator that does not cancel. The horizontal asymptote comes from comparing degrees: top degree smaller gives y = 0, equal degrees gives y = ratio of leading coefficients.

## Transformations and composition

**Transformation table.** Memorize this one.

| Change | What happens |
| --- | --- |
| f(x) + k | up k |
| f(x) − k | down k |
| f(x + h) | left h (the opposite of what it looks like) |
| f(x − h) | right h |
| c · f(x), c > 1 | stretch vertically |
| c · f(x), 0 < c < 1 | squash vertically |
| f(cx), c > 1 | squash horizontally |
| −f(x) | flip over the x-axis |
| f(−x) | flip over the y-axis |

Worked example: y = −2(x + 3)² + 5 from y = x². Left 3, stretch by 2, flip over the x-axis, up 5. The vertex moves from (0, 0) to (−3, 5), and it opens down.

**Matching graphs by asymptote.** The asymptote moves with the graph, so find it first.

| Function | Vertical asymptote | Horizontal asymptote |
| --- | --- | --- |
| 1/(x − 4) | x = 4 | y = 0 |
| 1/x + 4 | x = 0 | y = 4 |
| 1/(x − 4) + 5 | x = 4 | y = 5 |
| 5ˣ + 3 | none | y = 3, rising |
| 5ˣ⁻³ | none | y = 0, shifted right 3 |
| 5ˣ⁺¹ − 4 | none | y = −4, shifted left 1 |
| 5⁻ˣ | none | y = 0, falling (flipped over the y-axis) |

**Combining functions.** Sum, difference and product have the domain where both functions work. A quotient also needs the bottom function ≠ 0.

**Composition.** (f ∘ g)(x) = f(g(x)). Put g into f, working inside out. The domain is every x that works in g, where g(x) also works in f.

Worked example: f(x) = √(x + 1) and g(x) = 3x − 4.

```latex
(f\circ g)(x) = \sqrt{(3x-4)+1} = \sqrt{3x-3}, \quad 3x-3 \ge 0 \Rightarrow [1, \infty)
```

```latex
(g\circ f)(x) = 3\sqrt{x+1} - 4, \quad x+1 \ge 0 \Rightarrow [-1, \infty)
```

The order matters: f ∘ g and g ∘ f are usually different.

**Triple composition.** f(x) = 6x² + 7, g(x) = 7x³, h(x) = 1/(4x). To find f(g(h(4))), start from the inside: h(4) = 1/16. Then g(1/16) = 7/4096. Then f(7/4096) = 6 · (7/4096)² + 7 = 147/8388608 + 7, about 7.0000175.

**Difference quotient.** For f(x) = 3 − 7x + 8x², expand f(a + h) with (a + h)² = a² + 2ah + h² (three terms, never two).

```latex
f(a+h) = 8a^2 + 16ah + 8h^2 - 7a - 7h + 3
```

Subtract f(a). Everything without an h cancels, leaving 16ah + 8h² − 7h. Divide each term by h:

```latex
\frac{f(a+h)-f(a)}{h} = 16a + 8h - 7
```

## Inverse functions

**One-to-one.** A function has an inverse only if no output repeats. Horizontal line test: every horizontal line crosses the graph at most once. x² fails on all reals (2 and −2 both give 4), but passes if you restrict to x ≥ 0, which is how √x becomes its inverse.

**What an inverse does.** It undoes the function: f⁻¹(b) = a exactly when f(a) = b. Inputs and outputs swap roles.

- If f(2) = −9, then f⁻¹(−9) = 2.
- Domain of f⁻¹ = range of f. Range of f⁻¹ = domain of f.
- The graph of f⁻¹ is the graph of f reflected over the line y = x.

**The 3-step method.**

1. Write y = f(x).
2. Swap x and y.
3. Solve for y. That is f⁻¹(x).

**Worked example 1.** f(x) = 2x + 1. Swap: x = 2y + 1. Solve: y = (x − 1) / 2.

**Worked example 2.** g(x) = 13x³ − 1. Swap: x = 13y³ − 1. Solve: y³ = (x + 1) / 13, so y is the cube root of (x + 1) / 13.

**Worked example 3.** h(x) = 2 / (x + 1). Swap: x = 2 / (y + 1). Then x(y + 1) = 2, so y + 1 = 2/x and y = 2/x − 1.

**Worked example 4 (the one with a domain question).**

```latex
f(x) = \frac{x}{4x+8}
```

Swap: x = y / (4y + 8). Multiply out: 4xy + 8x = y. Collect the y terms: 8x = y − 4xy = y(1 − 4x). So:

```latex
f^{-1}(x) = \frac{8x}{1-4x}
```

| Quantity | Value | How to see it |
| --- | --- | --- |
| Domain of f | x ≠ −2 | denominator 4x + 8 ≠ 0 |
| Range of f | y ≠ 1/4 | f gets close to 1/4 for huge x but never equals it |
| Domain of f⁻¹ | x ≠ 1/4 | denominator 1 − 4x ≠ 0, and it equals the range of f |
| Range of f⁻¹ | y ≠ −2 | it equals the domain of f |

**Worked example 5.** f(x) = √(x² + 2x), x > 0. Square both sides of y = √(x² + 2x) to get y² = x² + 2x. Add 1: y² + 1 = (x + 1)². Now swap x and y: x² + 1 = (y + 1)², so f⁻¹(x) = √(x² + 1) − 1.

**Worked example 6.** f(x) = 8x⁵ + 6x + 6. Find x when f⁻¹(x) = −1. That means f(−1) = x, so x = −8 − 6 + 6 = −8. No algebra needed.

## Trigonometry

**Radians and degrees.** radians = degrees × π/180, and degrees = radians × 180/π. So 210° = 7π/6, and π/5 = 36°.

**Unit circle.** The point at angle t is P(t) = (cos t, sin t). The x-coordinate is cosine, the y-coordinate is sine. Learn the first-quadrant row, then get every other angle from its reference angle and the sign rule.

| t | 0 | π/6 | π/4 | π/3 | π/2 |
| --- | --- | --- | --- | --- | --- |
| sin t | 0 | 1/2 | √2/2 | √3/2 | 1 |
| cos t | 1 | √3/2 | √2/2 | 1/2 | 0 |
| tan t | 0 | √3/3 | 1 | √3 | undefined |

**Signs by quadrant (All Students Take Calculus).** Quadrant I: all positive. II: only sin (and csc). III: only tan (and cot). IV: only cos (and sec).

**Method for any angle.**

1. Subtract 2π until the angle is between 0 and 2π.
2. Find the quadrant, then the reference angle (distance to the x-axis).
3. Use the first-quadrant value and the sign for that quadrant.

Quadrants: 2π/3 is in II. 11π/4 − 2π = 3π/4 is in II. 23π/6 − 2π = 11π/6 is in IV. 5 radians is about 286.5°, so IV.

Worked example: −5π/6 points into quadrant III with reference angle π/6. There sin and cos are negative and tan is positive. So sin = −1/2, cos = −√3/2, tan = √3/3, sec = −2√3/3.

**Points to memorize (every multiple of π/4 on the axes and diagonals).**

| t | 0 | π/4 | π/2 | 3π/4 | π | 5π/4 | 3π/2 | 7π/4 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| sin t | 0 | √2/2 | 1 | √2/2 | 0 | −√2/2 | −1 | −√2/2 |
| cos t | 1 | √2/2 | 0 | −√2/2 | −1 | −√2/2 | 0 | √2/2 |

**Symmetry moves.** If P(t) = (c, s), then:

| Angle | Point |
| --- | --- |
| −t | (c, −s) |
| t + π and t − π | (−c, −s) |
| −t − π | (−c, s) |

**Identities.**

```latex
\sin^2\theta + \cos^2\theta = 1, \qquad 1 + \tan^2\theta = \sec^2\theta, \qquad 1 + \cot^2\theta = \csc^2\theta
```

csc = 1/sin, sec = 1/cos, cot = 1/tan. cos and sec are even. sin, tan, csc and cot are odd.

**Worked example.** sin u = 3/5 and cos u is negative, so u is in II. From a 3-4-5 triangle, cos u = −4/5 and tan u = −3/4. Then sin(−u) = −3/5, cos(−u) = −4/5, tan(−u) = 3/4. Adding π flips sin and cos: sin(u + π) = −3/5, cos(u + π) = 4/5, and tan(u + π) = −3/4 (tan repeats every π). Adding π/2 swaps them: sin(u + π/2) = cos u = −4/5, cos(u + π/2) = −sin u = −3/5, tan(u + π/2) = −cot u = 4/3.

**Exact values from one ratio.** cos θ = 1/8 in quadrant I. Then sin θ = √(1 − 1/64) = 3√7 / 8. So csc θ = 8√7 / 21 and cot θ = √7 / 21.

**Right triangles.** Before using SOH-CAH-TOA, find which angle you are measuring. Opposite is the side across from that angle. In a 9-40-41 triangle, if the angle sits where the 41 meets the 9, then opposite = 40, so sin = 40/41 and cos = 9/41.

**Solving equations.**

- sin x = −1/2 on \[0, 2π): the reference angle is π/6 and sin is negative in III and IV, so x = 7π/6 and 11π/6.
- tan t = 3 / tan t: multiply by tan t to get tan²t = 3, so tan t = ±√3 and t = π/3, 2π/3, 4π/3, 5π/3.

**Graphs of sin and cos.** For A sin(B(x − C)) + D:

```latex
\text{amplitude} = |A|, \quad \text{period} = \frac{2\pi}{|B|}, \quad \text{shift} = C, \quad \text{midline } y = D
```

Max = D + |A|, min = D − |A|. Example: 3 sin((π/6)(x − 5)) − 4 has amplitude 3, period 12, max −1 and min −7. To tell the basic graphs apart: sin starts at 0 and rises, cos starts at 1 and falls, and tan has vertical asymptotes at π/2 + kπ.

## Inverse trig

sin, cos and tan repeat forever, so they are not one-to-one. To invert them we cut each one down to a stretch where it is one-to-one. The inverse then gives back the angle from that stretch.

**Memorize this table.**

| Function | Domain (inputs) | Range (output angle) |
| --- | --- | --- |
| arcsin x | \[−1, 1\] | \[−π/2, π/2\] |
| arccos x | \[−1, 1\] | \[0, π\] |
| arctan x | all reals | (−π/2, π/2) |

arcsin x means: the angle between −π/2 and π/2 whose sine is x. The answer must land in that range, which decides between look-alike angles.

**Worked examples.**

| Expression | Answer | Reason |
| --- | --- | --- |
| arcsin(√2/2) | π/4 | sin(π/4) = √2/2 |
| arcsin(0) | 0 | sin 0 = 0 |
| arcsin(−√2/2) | −π/4 | negative angles are allowed for arcsin |
| arccos(0) | π/2 | cos(π/2) = 0 |
| arccos(−1/2) | 2π/3 | must be in \[0, π\], so quadrant II, not III |
| arctan(1) | π/4 | tan(π/4) = 1 |
| arctan(−1) | −π/4 | tan(−π/4) = −1 |

**Domain and range of arcsin(3x + 1).** The inside must be in \[−1, 1\]: −1 ≤ 3x + 1 ≤ 1, so −2 ≤ 3x ≤ 0, so −2/3 ≤ x ≤ 0. The range stays −π/2 ≤ y ≤ π/2.

**The trap.** arcsin(sin x) equals x only when x is already in \[−π/2, π/2\]. For g(x) = arcsin(sin x) on \[0, 2π\], g(x) = 0 wherever sin x = 0, which is x = 0, π and 2π.

**Triangle method.** To simplify something like cos(arctan x):

1. Let θ = arctan x, so tan θ = x = x/1.
2. Draw a right triangle with opposite = x, adjacent = 1, so hypotenuse = √(x² + 1).
3. Read off the ratio you want, and check the sign using the range of θ.

```latex
\cos(\arctan x) = \frac{1}{\sqrt{x^2+1}}
```

The sign is positive because arctan gives angles in (−π/2, π/2), where cosine is positive.

For sin(arcsec x): let θ = arcsec x, so cos θ = 1/x and θ is in \[0, π\], where sine is never negative. So sin θ = √(1 − 1/x²), which simplifies to:

```latex
\sin(\operatorname{arcsec} x) = \frac{\sqrt{x^2-1}}{|x|}
```

**Recognizing the graphs.** arcsin rises from (−1, −π/2) through the origin to (1, π/2). arccos falls from (−1, π) through (0, π/2) down to (1, 0). arctan is an S-curve over all x that flattens out near π/2 on the right and −π/2 on the left.

## Exponentials, logarithms and modeling

|  | Exponential aˣ (a > 0, a ≠ 1) | Logarithm logₐ x |
| --- | --- | --- |
| Domain | all reals | x > 0 |
| Range | y > 0 | all reals |
| Asymptote | horizontal, y = 0 | vertical, x = 0 |
| Key point | (0, 1) | (1, 0) |
| Shape | rises if a > 1, falls if 0 < a < 1 | rises if a > 1, falls if 0 < a < 1 |

They are inverses: y = logₐ x means exactly aʸ = x. "log" with no base is base 10, and ln is base e. Both 2ˣ and log₂ x rise. Both (1/2)ˣ and log base 1/2 of x fall.

**Log rules.**

```latex
\log_a(xy) = \log_a x + \log_a y, \qquad \log_a\frac{x}{y} = \log_a x - \log_a y, \qquad \log_a(x^r) = r\log_a x
```

```latex
\log_a a = 1, \qquad \log_a 1 = 0, \qquad a^{\log_a x} = x, \qquad \log_a x = \frac{\ln x}{\ln a}
```

**Domains with eˣ.** 1/(1 + eˣ): the bottom is always bigger than 1, so the domain is all reals. 1/(1 − eˣ): the bottom is 0 when eˣ = 1, which happens at x = 0, so x ≠ 0.

**Solving exponential equations.**

- Same base: 16ˣ = 64 becomes (2⁴)ˣ = 2⁶, so 4x = 6 and x = 3/2. Likewise 9ˣ⁺¹ = 27 gives 3²ˣ⁺² = 3³, so x = 1/2.
- Otherwise take a log of both sides. e²ˣ⁺³ = 4 gives 2x + 3 = ln 4, so x = (ln 4 − 3) / 2.
- 10ˣ⁻⁵ = 6 gives x − 5 = log 6, so x = 5 + log₁₀ 6.

**Solving log equations.** Rewrite as an exponential, solve, then check the answer is inside the log's domain.

| Equation | Steps | Answer |
| --- | --- | --- |
| ln(5 − 2x) = −2 | 5 − 2x = e⁻² | x = (5 − e⁻²) / 2 |
| ln(3x + 6) = 4 | 3x + 6 = e⁴ | x = (e⁴ − 6) / 3 |
| log₁₀(3x − 5) = 3 | 3x − 5 = 1000 | x = 335 |
| log₂ x + log₂(x − 2) = 3 | x(x − 2) = 8, so (x − 4)(x + 2) = 0 | x = 4 (reject −2, it makes x − 2 negative) |
| ln x + ln(x − 1) = 1 | x(x − 1) = e, so x² − x − e = 0 | x = (1 + √(1 + 4e)) / 2 (reject the negative root, need x > 1) |

In WebWork, log(x) means the natural log. Type log10(x) for base 10.

**Modeling with exponentials.** A quantity that multiplies by 2 every T hours, starting at P₀, is P(t) = P₀ · 2^(t/T). Worked example: 100 bacteria doubling every 3 hours.

```latex
P(t) = 100 \cdot 2^{t/3}
```

After 9 hours: 100 · 2³ = 800. After 19 hours: 100 · 2^(19/3), about 8063.5. A constant amount added per step is a linear model (y = mx + b). A constant multiplier per step is exponential.

## Practice test

Solve these on paper with the guide closed, then check the key below. Each one uses new numbers, so you cannot just copy a worked example.

1. Find the domain of f(x) = √(2x − 6) / (x − 5).
2. Solve −3x + 9 > 0 and write the answer in interval notation.
3. Find the range of f(x) = −x² + 4.
4. Even, odd or neither? (a) x³ − 5x. (b) x⁴ + x.
5. For f(x) = 2x² − 12x + 7, find the vertex and say whether it is a minimum or maximum.
6. Describe how to get y = −(x − 2)² + 1 from y = x².
7. Let f(x) = x² + 1 and g(x) = √(x − 2). Find f(g(x)) and its domain.
8. Find the inverse of f(x) = (3x − 1) / (x + 2), and state the domain of f⁻¹.
9. Evaluate sin(5π/4), cos(−π/3) and tan(2π/3).
10. sin θ = −4/5 and θ is in quadrant III. Find cos θ and tan θ.
11. Find the amplitude, period and maximum of y = 2 cos(3x) + 1.
12. Solve 2 cos t = −√3 for 0 ≤ t < 2π.
13. Evaluate arccos(√3/2), arcsin(−1) and cos(arcsin(3/5)).
14. Solve (a) 5^(2x − 1) = 125. (b) ln x + ln(x + 2) = ln 8.
15. A population of 400 triples every 2 hours. Write P(t) and find the population after 6 hours.

**Answer key**

| Q | Answer | Key step |
| --- | --- | --- |
| 1 | \[3, 5) ∪ (5, ∞) | 2x − 6 ≥ 0 gives x ≥ 3, and x ≠ 5 |
| 2 | (−∞, 3) | −3x > −9, divide by −3 and flip: x < 3 |
| 3 | (−∞, 4\] | frown with highest point 4 |
| 4 | (a) odd, (b) neither | (a) only odd powers. (b) mixes even and odd powers |
| 5 | vertex (3, −11), minimum −11 | x = 12/4 = 3, f(3) = 18 − 36 + 7 = −11, and a > 0 |
| 6 | right 2, flip over the x-axis, up 1 | vertex (2, 1), opens down |
| 7 | f(g(x)) = x − 1, domain \[2, ∞) | (√(x − 2))² + 1 = x − 1, but g needs x ≥ 2 |
| 8 | f⁻¹(x) = (2x + 1) / (3 − x), domain x ≠ 3 | x(y + 2) = 3y − 1, so 2x + 1 = y(3 − x) |
| 9 | −√2/2, 1/2, −√3 | quadrant III, cos is even, quadrant II |
| 10 | cos θ = −3/5, tan θ = 4/3 | 3-4-5 triangle, both legs negative in III |
| 11 | amplitude 2, period 2π/3, max 3 | 2π/3 from 2π/B, max = 1 + 2 |
| 12 | t = 5π/6, 7π/6 | cos t = −√3/2, reference angle π/6, negative in II and III |
| 13 | π/6, −π/2, 4/5 | triangle with opposite 3, hypotenuse 5, adjacent 4 |
| 14 | (a) x = 2. (b) x = 2 | (a) 2x − 1 = 3. (b) x² + 2x = 8, so (x + 4)(x − 2) = 0, reject −4 |
| 15 | P(t) = 400 · 3^(t/2), then 10,800 | 6 hours is 3 triplings: 400 · 27 |

For every question you missed, go back to its section, redo the worked example without looking, then retry the question.
