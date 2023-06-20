## Solve the problem of hiding a point in a 3D plot

### Problem: A point gets hidden in a surface plot.
### Solution:
Use `computed_zorder` to be `False while creating figure.

Here is an example 👇
```python
fig: plt.Figure
ax: Axes3D
fig, ax = plt.subplots(subplot_kw={"projection": "3d", "computed_zorder": False})

# A point
ax.scatter(10,70,4, c='k', depthshade=False, alpha = 1, s=100)

# Surface plot
surf = ax.plot_surface(yv,xv,df, cmap='viridis_r', linewidth=0.3,
                       alpha = 0.8, edgecolor = 'k', norm=norm)

# Another point
ax.scatter(25,35,4, c='k', depthshade=False, alpha = 1, s=100)

plt.show()
```
