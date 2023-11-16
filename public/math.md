### Problem 1: $$f(x)=x^4+3x^2+6e^x$$

To find the derivative f′(x), we apply the power rule to each term where the derivative of x^n is nx^(n-1), and the derivative of e^x is e^x
$$
f'(x) = \frac{d}{dx}(x^4) + \frac{d}{dx}(3x^2) + \frac{d}{dx}(6e^x)
f'(x) = 4x^3 + 6x + 6e^x
$$

### Problem 2: $$g(x)=sin(3e^x)$$

For g(x), we use the chain rule, where the derivative of sin(u) is cos(u)⋅u′.

$$g'(x) = \frac{d}{dx}(\sin(3e^x))
Let \, u = 3e^x \Rightarrow u' = 3e^x
g'(x) = \cos(u) \cdot u' = \cos(3e^x) \cdot 3e^x
g'(x) = 3e^x \cos(3e^x)
$$

### Problem 3: $$y=x^2cos(x^3−3)$$

For y, the product rule is needed, which is (uv)′=u′v+uv′, and also the chain rule for the cosine part.

$$y' = \frac{d}{dx}(x^2) \cdot \cos(x^3 - 3) + x^2 \cdot \frac{d}{dx}(\cos(x^3 - 3))
y' = 2x \cos(x^3 - 3) - x^2 \sin(x^3 - 3) \cdot 3x^2
y' = -3x^4 \sin(x^3 - 3) + 2x \cos(x^3 - 3)
$$

Problem 4: $$\frac{dx}{d}​\frac{e^x}{(tan(x^2+4​)}$$
$$Let \, u = e^x \, and \, v = \tan(x^2 + 4)
u' = e^x \, and \, v' = \sec^2(x^2 + 4) \cdot 2x = 2x(\tan^2(x^2 + 4) + 1)

\frac{d}{dx} \left( \frac{e^x}{\tan(x^2 + 4)} \right) = \frac{e^x \cdot \tan(x^2 + 4) - e^x \cdot 2x(\tan^2(x^2 + 4) + 1)}{\tan^2(x^2 + 4)}
\frac{d}{dx} \left( \frac{e^x}{\tan(x^2 + 4)} \right) = \frac{e^x}{\tan(x^2 + 4)} - \frac{2x(\tan^2(x^2 + 4) + 1)e^x}{\tan^2(x^2 + 4)}
$$


You are constructing an open-top box with a square base for your dog to sleep in. You need a box with a volume of 4ft^3. Find the dimensions of the box that will minimize the amount of material used. Use x to represent the side length of the square base and ℎh to represent the height of the box."

To solve this, we'll perform the following steps:

1. Express the volume of the box in terms of x and h.
2. Use the volume requirement to find a relationship between x and h.
3. Express the surface area of the box, which represents the material used, in terms of a single variable.
4. Differentiate the surface area to find the minimum.

$$
\text{Step 1: Volume Equation } \\
V = x^2h \quad \text{where } x \text{ is the side length and } h \text{ is the height.}
$$

$$
\text{Step 2: Given Volume } \\
x^2h = 4 \quad \text{(Volume of the box is } 4ft^3 \text{)}
$$
$$
\text{Step 3: Solve for } h \text{ in terms of } x, \\
h = \frac{4}{x^2}
$$
$$
\text{Step 4: Surface Area Equation for an open-top box } \\
SA = x^2 + 4(xh) \quad \text{(Only the base and the sides contribute to the surface area)}
$$
$$
\text{Step 5: Substitute } h \text{ into the Surface Area Equation } \\
SA = x^2 + \frac{16}{x}
$$
$$
\text{Step 6: Differentiate SA with respect to } x ,\\
\frac{d(SA)}{dx} = 2x - \frac{16}{x^2}
$$
$$
\text{Step 7: Find Critical Points } \\
2x - \frac{16}{x^2} = 0
$$
$$
\text{Step 8: Solve for } x, \\
x = 2 \, ft
$$
$$
\text{Step 9: Calculate } h \text{ using the value of } x ,  \\
h = \frac{4}{x^2} = 1 \, ft
$$
$$
\text{Step 10: Confirm Minimum Surface Area, } \\
SA = x^2 + \frac{16}{x} = 4 + 8 = 12 \, ft^2
$$


"A farmer is constructing a large rectangular pen to hold three llamas, with two internal separation fences so that there is one smaller pen for each llama. The two internal separation fences are parallel to one side of the larger pen. The farmer has 900 meters of fence material for this project. What is the maximum total area of all three pens?"

1. Define variables for the dimensions of the pens.
2. Write an equation for the perimeter of the pens using the available fence material.
3. Express the total area of the pens in terms of a single variable.
4. Use differentiation to find the maximum area.

The dimensions of the pens that will maximize the total area, given 900 meters of fence material, are:

- Width of each smaller pen (w): 150150 meters
- Length of the entire set of pens (l): 225225 meters

The maximum total area of all three pens combined is 33,75033,750 square meters.

$$
P = 2l + 3w = 900 \quad \text{where } l \text{ is the length and } w \text{ is the width of the entire pen.}
$$

$$
l = \frac{900 - 3w}{2}
$$

$$
A = l \cdot w
$$
$$
A = \left(\frac{900 - 3w}{2}\right)w
$$
$$
\frac{dA}{dw} = \frac{900}{2} - 3w
$$
$$
\frac{900}{2} - 3w = 0
$$
$$
w = 150 \, m
$$
Calculate l using the maximum value of w.
$$
l = \frac{900 - 3(150)}{2} = 225 \, m
$$
Calculate the maximum total area using the values of l and w.
$$
A_{max} = 225 \cdot 150 = 33,750 \, m^2
$$
