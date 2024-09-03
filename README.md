# typster-scripts

## tabler

скрипт для создания таблиц истиности (note: `<=` тоде самое что `xor` | `->` )
```sh
$ ./tabler "lambda x, y, z: x and y <= z"
```

```typ
#let fal = table.cell(
  fill: red.lighten(60%)
)[False]

#let tru = table.cell(
  fill: green.lighten(60%)
)[False]

#table(
    columns: 4,
    stroke: 0.5pt,
    align: center+ horizon,
    [x], [y], [z], [$x and y -> z$],
    fal, fal, fal, fal, fal, fal, tru, fal, fal, tru, fal, fal, fal, tru, tru, fal, tru, fal, fal, tru, tru, fal, tru, tru, tru, tru, fal, fal, tru, tru, tru, tru
)
```
