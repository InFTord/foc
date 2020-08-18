## Common
inherit - значение от родителя
initial - значение по умолчанию в браузере
unset - значение от родителя, если оно есть, либо по умолчанию

### units - еденица измерения
[
  px - один пиксел
  in - 96px
  cm - 96px/2.54
  mm - 96px/25.4
  pt - 96px/72
  pc - 16px
] | [
  vh - 1/100 высоты
  vw - 1/100 ширины
  vi - 1/100 исходного блока в inline
  vb - 1/100 исходного блока в block
  vmin - min(vw, vh)
  vmax - max(vw, vh)
] | [
  ch - ширина "0", либо 1em x 0.5em
  em - размер шрифта элемента
  ex - высота "x"
  rem - размер шрифта html
]

### number - рациональные числа

### integer - целые числа

### percentage - процент относительно родителя
[number]%

### length - длина
[number][units]

### width - ширина
[length] | [percentage]
auto - автоматически
max-content - предпочтительная
min-content - собственная минимальная
fit-content - min([max-content], max([min-content], [length | percentage]))

### display - отображение
[
  block - занимает полностью строку
  inline - следующий элемент в той же строке, если есть место
] || [
  flow-root - отдельный block контекст форматирования
  table - как <table>, сам block
  inline-table - как <table>, сам inline
  flex - модель Flexbox, сам block
  inline-flex - модель Flexbox, сам inline
  grid - модель Grid, сам block
  inline-grid - модель Grid, сам inline
]

inline-block - как одиночный inline элемент
[
  list-item - как элемент списка
] || [block | inline] || [flow | flow-root]

table-row-group - как <tbody>
table-header-group - как <thead>
table-footer-group - как <tfoot>
table-row - как <tr>
table-cell - как <td>
table-column-group - как <colgroup>
table-column - как <col>
table-caption - как <caption>

contents - не отображается, дерево переходит к родителю
none - не отображается дерево элементов

## Grid
### grid
[grid-template-rows] || [grid-template-columns] || [grid-template-areas]
[grid-auto-rows] || [grid-auto-columns] || [grid-auto-flow]
### grid-template-rows - определяет имена линий и функции определения размера grid rows.
### grid-template-columns
### grid-template - определения столбцов, строк и областей сетки