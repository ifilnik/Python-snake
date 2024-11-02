# Яблочная змея

Яблочная змея - это увлекательная игра, где вы управляете змейкой, собирая яблоки, чтобы она росла. Цель игры - съесть как можно больше яблок, избегая столкновений со стенами или с телом змейки.

## Установка

1. Убедитесь, что у вас установлены Python и Pygame:
   - Скачайте и установите Python с [python.org](https://www.python.org/).
   - Установите Pygame, введя следующую команду в командной строке:
    
  ```pip install pygame```
     
2. Скачайте игру:
   - Скачайте файл игры snake_game.py

3. Запустите игру:
  
   ```python snake_game.py```
   
## Как играть

- Управление змейкой:
  - Используйте клавиши со стрелками для управления направлением движения змейки:
    - Нажмите вверх, чтобы двигаться вверх.
    - Нажмите вниз, чтобы двигаться вниз.
    - Нажмите влево, чтобы двигаться влево.
    - Нажмите вправо, чтобы двигаться вправо.

- Сбор яблок:
  - Змейка растет с каждым съеденным яблоком.
  - Яблоки могут быть оранжевого или красного цвета, выбираются случайным образом.

- Избегайте препятствий:
  - Избегайте столкновений со стенами окна игры.
  - Избегайте столкновений с телом змейки.

## Функционал игры

1. Импорт и инициализация:
   - Импортируются библиотеки Pygame и random.
   - Инициализируются модули Pygame с помощью `pygame.init().`

2. Настройки экрана и цветов:
   - Устанавливаются цвет фона, размеры окна и заголовок окна.
   - Задаются цвета змейки и яблок, выбирается случайный цвет яблока.

3. Начальные параметры змейки и яблока:
   - Устанавливаются начальные координаты сегментов змейки и направление её движения.
   - Генерируется случайная начальная позиция яблока.
   - Устанавливается начальный счет.

4. Игровой цикл:
   - Запускается основной цикл игры, который продолжается, пока `running = True.`
   - Обрабатываются события, такие как выход из игры и нажатия клавиш для управления направлением движения змейки.

5. Обновление позиции змейки:
   - Определяется новая позиция головы змейки в зависимости от текущего направления движения (вверх, вниз, влево, вправо).

6. Обработка столкновений и обновление состояния:
   - Проверяется, съела ли змейка яблоко. Если да, то увеличивается счет, и генерируется новая позиция яблока.
   - Если яблоко не съедено, удаляется последний сегмент змейки.
   - Добавляется новая голова змейки в начало списка сегментов.

7. Проверка на проигрыш:
   - Проверяется столкновение змейки с границами экрана или с собственным телом. Если произошло столкновение, игра завершается.

8. Отрисовка экрана:
   - Заполняется фон цветом.
   - Отрисовываются сегменты змейки и яблоко.

9. Завершение работы:
   - Завершается работа Pygame с помощью `pygame.quit().`

## Особенности игры

- Цвета яблок: Два варианта яблок: оранжевые и красные.
- Интуитивный геймплей: Легкое управление, подходящее для всех возрастов.
- Подсчет очков: Ведется счет съеденных яблок.
- Гибкость настроек: Возможность изменить параметры игры, такие как скорость передвижения "змейки", размер экрана и цветовые схемы, редактируя код.

## Зависимости

- Python 3.x: Необходим для запуска игры.
- Pygame: Библиотека для создания игр на Python.

## Лицензия

Этот проект лицензирован по лицензии MIT. Подробности можно найти в файле LICENSE.
