## CSS Grid Course

Tutorial base from [FreeCodeCamp youtube]('https://www.youtube.com/watch?v=t6CBKf8K_Ac&t=62s')

- ⌨️ 0:01 1. Course Introduction
- ⌨️ 4:47 2. Your first grid
- ⌨️ 8:03 3. Fraction units and repeat
- ⌨️ 11:45 4. Positioning items
- ⌨️ 18:28 5. Template areas
- ⌨️ 23:18 6. Auto-fit and minmax
- ⌨️ 27:07 7. Implicit rows
- ⌨️ 29:06 8. An awesome image grid
- ⌨️ 35:56 9. Bonus: Named Lines
- ⌨️ 41:25 10. Bonus: Justify-content and align-content
- ⌨️ 44:17 11. Bonus: Justify-items and align-items
- ⌨️ 47:44 12. Bonus: Auto-fit vs. auto-fill
- ⌨️ 49:39 13. Bonus: Creating an article layout
- ⌨️ 57:37 14. Bonus: Grid vs. Flexbox

## First Grid

style.css

```
.container {
  display: grid;
  grid-template-columns: 50px auto 50px;
  grid-template-rows: 50px 50px;
  gap: 5px;
}
```

> display : grid;

- defines the elements as a grid container and establishes a new grid formatting context for its content
  <br>

> grid-template-colums <br>
> grid-template-rows

- defines the columns and rows of the grid with a space-separated list of values.The values represent the track size, and the space between them represents the grid line.

## Fraction units and repeat
style.css
```
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 1fr);
  gap: 5px;
}
```
short-hand
```
.container {
  display: grid;
  grid-template: repeat(2, 1fr)/ repeat(3, 1fr);
  gap: 5px;
}

```

> fr units
- they essentially mean "portion of the remaining space".
> repeat
- represent a repeated fragment of the track list, allowing a large number of columns or rows that exhibit a recurring pattern to be written in a more compact form.

## Postioning items