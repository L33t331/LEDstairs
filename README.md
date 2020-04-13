# LEDstairs
Контроллер подсветки лестницы на Arduino  

## Новые функции в прошивке 1.1
1) поддержка **ночного режима**. Подсвечиваются крайние ступеньки.
  Настройка:
  * маска (какие диоды на ступеньке включать) NIGHT_LIGHT_BIT_MASK
  * цвет NIGHT_LIGHT_COLOR
  * яркость NIGHT_LIGHT_BRIGHT

```c
#define NIGHT_LIGHT_BIT_MASK 0b1000000100000001  // последовательность диодов в ночном режиме
#define NIGHT_LIGHT_COLOR 50  // 0 - 255
#define NIGHT_LIGHT_BRIGHT 50  // 0 - 255
```
Чтобы не выжигать одни и теже диоды, маска сдвигается на один диод вправо каждые 15 секунд  
  
2) включение только при минимальной освещённости

Автор: Геннадий Дегтерёв  
gennadij@degterjow.de


* Основная страница оригинального проекта здесь https://alexgyver.ru/ledstairs/

