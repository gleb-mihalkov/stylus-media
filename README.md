# [В разработке] Stylus.Media

*Библиотека для генерации медиа-запросов на препроцессоре Stylus.*

## Использование

````bash
npm install --save {this-repo}
````

````stylus
@import 'node_modules/stylus-media/media'

body
  width 1280px
  margin 0 auto
  padding 0 80px

  +media-width-less-then(1280px)
    width 960px
    padding 0 40px

  +media-width-less-then(960px)
    width 480px
    padding 0 20px

  +media-width-less-then(480px)
    width 100%
````

## Описание API

### media-width-less-then(unit $value)

Генерирует медиа-запрос по условию "ширина экрана меньше указанного значения".

### media-width-less-eq-then(unit $value)

Генерирует медиа-запрос по условию "ширина экрана меньше или равна указанному значению".

### media-width-bigger-then(unit $value)

Генерирует медиа-запрос по условию "ширина экрана больше указанного значения".

### media-width-bigger-eq-then(unit $value)

Генерирует медиа-запрос по условию "ширина экрана больше или равна указанному значению".

### media-height-less-then(unit $value)

Генерирует медиа-запрос по условию "высота экрана меньше указанного значения".

### media-height-less-eq-then(unit $value)

Генерирует медиа-запрос по условию "высота экрана меньше или равна указанному значению".

### media-height-bigger-then(unit $value)

Генерирует медиа-запрос по условию "высота экрана больше указанного значения".

### media-height-bigger-eq-then(unit $value)

Генерирует медиа-запрос по условию "высота экрана больше или равна указанному значению".
