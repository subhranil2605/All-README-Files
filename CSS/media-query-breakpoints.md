# When using a web-first approach for responsive web design, the following media query breakpoints are commonly used

- Extra Small Devices (less than `576px`):

```css
@media (max-width: 575.98px) {
    /* Styles for extra small devices */ 
}
```

- Small Devices (`576px` to `767.98px`):

```css
@media (min-width: 576px) and (max-width: 767.98px) { 
    /* Styles for small devices */ 
}
```

- Medium Devices (`768px` to `991.98px`):

```css
@media (min-width: 768px) and (max-width: 991.98px) {
    /*Styles for medium devices*/ 
}
```

- Large Devices (`992px` to `1199.98`px):

```css
@media (min-width: 992px) and (max-width: 1199.98px) {
    /*Styles for large devices*/ 
}
```

- Extra Large Devices (`1200px` and above):

```css
@media (min-width: 1200px) {
    /*Styles for extra large devices*/ 
}
```

---
> These breakpoints are based on the Bootstrap      framework's default breakpoints, which are widely adopted in responsive web design.
However, it's important to note that breakpoints can vary depending on the specific design requirements of your project.
You can customize and add additional breakpoints based on your needs.
