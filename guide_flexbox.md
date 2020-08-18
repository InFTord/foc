## Flexbox
### flex-direction - направление
row (по умолчанию) - в строку
row-reverse - в строку, в обратном порядке
column - в столбец
column-reverse - в столбец, в обратном порядке

### flex-wrap - перенос
nowrap (по умолчанию) - в одну линию
wrap - на несколько строк
wrap-reverse - на несколько строк, в обратном порядке

### flex-flow
[flex-direction] || [flex-wrap]

### flex-grow - коэффициент гибкости
[+number] - число|0 (по умолчанию)

### flex-shrink - коэффициент сжатия
[+number] - число|1 (по умолчанию)

### flex-basis - начальный размер
[width] - значения width|auto (по умолчанию)
content - автоматический

### flex
[flex-grow|1] || [flex-shrink|1] || [flex-basis|0]
auto - 1 1 auto
none - 0 0 auto

### order - порядок
[integer] - номер места

### align-content - пространство между элементами вдоль поперечной оси
[
  normal (по умолчанию)
  baseline | first baseline | last baseline - линии, на которых "сидят" буквы
  space-between - крайние прижаты
  space-around - расстояние у крайних = 1/2 расстояния
  space-evenly - расстояние у крайних = 1 расстоянию
  stretch - все поля равны
] | [
  [
    safe - выравнивание за пределами
    unsafe - не зависит от пределов
  ] || [
    center - по центру
    start - элементы по началу
    end - элементы по концу
    flex-start - флекс элементы по началу
    flex-end - флекс элементы по концу
  ]
]

### align-items - выравнивание по поперечной оси
[
  normal (по умолчанию)
  baseline | first baseline | last baseline - линии, на которых "сидят" буквы
  stretch - все поля равны
] | [
  [
    safe - выравнивание за пределами
    unsafe - не зависит от пределов
  ] || [
    center - по центру
    start - элементы по началу
    end - элементы по концу
    flex-start - флекс элементы по началу
    flex-end - флекс элементы по концу
    self-start - элементы по началу по своей оси
    self-end - элементы по концу по своей оси
  ]
]

### align-self - выравнивание по поперечной оси отдельного элемента
center - по центру
flex-start - флекс элементы по началу
start - элементы по началу
flex-end - флекс элементы по концу
end - элементы по концу
baseline | first baseline | last baseline - линии, на которых "сидят" буквы
auto - по родительскому элементу

### justify-content - пространство между элементами вдоль главной оси
[
  normal (по умолчанию) - stretch
  left - все элементы слева
  right - все элементы справа
  space-between - крайние прижаты
  space-around - расстояние у крайних = 1/2 расстояния
  space-evenly - расстояние у крайних = 1 расстоянию
  stretch - все поля равны
] | [
  [
    safe - выравнивание за пределами
    unsafe - не зависит от пределов
  ] || [
    center - по центру
    start - элементы по началу
    end - элементы по концу
    flex-start - флекс элементы по началу
    flex-end - флекс элементы по концу
  ]
]