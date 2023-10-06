(Chap_SciPy)=
# SciPy

SciPy is Python's primary scientific computing package.[^SciPy] As described in the {ref}`Chap_NumPy` chapter, SciPy is built with NumPy as a core dependency. The SciPy website [homepage](https://scipy.org/) states that, "SciPy provides algorithms for optimization, integration, interpolation, eigenvalue problems, algebraic equations, differential equations, statistics and many other classes of problems."

The `OG-Core` model and its country calibrations use SciPy primarily for three things, although there are some other smaller use cases.
* Finding the roots or zeros of functions ([`scipy.optimize.root`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.root.html))
* Solving minimization problem ([`scipy.optimize.minimize`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html))
* Interpolation ([`scipy.interpolate`](https://docs.scipy.org/doc/scipy/tutorial/interpolate.html))


(Sec SciPyRoot)=
## Root finding


(SecSciPyMin)=
## Minimization


(SecSciPyInterp)=
## Interpolation


(SecSciPyExercises)=
## Exercises

```{exercise-start}
:label: ExerScipy-root_save
```
Define household FOC for savings and use `scipy.optimize.root` to solve for the optimal savings rate for a household with CRRA utility
```{exercise-end}
```

```{exercise-start}
:label: ExerScipy-root_labor
```
Define the household FOC for labor supply and use `scipy.optimize.root` to solve for the optimal labor supply for a household with ellipitcal utility
```{exercise-end}
```

```{exercise-start}
:label: ExerScipy-min
```
Use `scipy.optimize.minimize` to minimize the function $f(x) = x^2 + 2x + 1$ (or some other function).
```{exercise-end}
```

```{exercise-start}
:label: ExerScipy-min_constraint
```
Use `scipy.optimize.minimize` to minimize the function $f(x) = x^2 + 2x + 1$ (or some other function) subject to the constraint that $x \geq 2$.
```{exercise-end}
```

```{exercise-start}
:label: ExerScipy-interp
```
Use `scipy.interpolate`...
```{exercise-end}
```


(SecSciPyFootnotes)=
## Footnotes

The footnotes from this chapter.

[^SciPy]: The website for Python's SciPy package is https://scipy.org.
