<h1 align="center">Звіт з лабораторної роботи №3</h1>
<h2 align="center">Реалізація перетворень між системами координат</h2>

<div align="center">
  <a href="https://codepen.io/pienovakatya/full/xbKVMOv" target="_blank">
    <img style="width: 300%; height: 300%;" src="https://img.shields.io/badge/CodePen-000000?style=for-the-badge&logo=codepen&logoColor=white" alt="Open in CodePen"/>
  </a>
</div>

## Мета роботи
Ознайомитися з різними системами координат (декартовою, полярною та сферичною) та отримати практичні навички у переході між ними. Визначити обчислювальну ефективність розрахунку відстаней у цих системах координат через бенчмаркінг.

## Завдання роботи
Реалізація програмного забезпечення для роботи з різними системами координат включала наступні аспекти: перетворення між декартовою та полярною системами координат у двовимірному просторі, перетворення між декартовою та сферичною системами координат у тривимірному просторі, а також розрахунок відстаней між точками різними методами. Окремою частиною роботи було проведення бенчмаркінгу для оцінки ефективності різних методів обчислення.

## Реалізація проєкту

### Початковий інтерфейс
Розроблений веб-додаток надає користувачу три основні функціональні блоки для роботи з координатами.

<p align="center">
  <img src="Screenshots/1.PNG" alt="1"/>
</p>
<p align="center">Головний екран програми з трьома функціональними блоками: перетворення координат, розрахунок відстаней та тестування продуктивності</p>

### Перетворення координат
Система автоматично виконує перетворення введених координат між різними системами, забезпечуючи точність обчислень та зручність використання.

<p align="center">
  <img src="Screenshots/2.PNG" alt="2"/>
</p>
<p align="center">Демонстрація результатів перетворення координат між полярною та декартовою системами</p>

### Розрахунок відстаней
Програма пропонує різні методи обчислення відстаней, враховуючи особливості кожної системи координат.

<p align="center">
  <img src="Screenshots/3.PNG" alt="3"/>
</p>
<p align="center">Візуалізація результатів обчислення відстаней різними методами для заданих точок</p>

### Тестування продуктивності
Проведено комплексне тестування продуктивності на значній вибірці даних для оцінки ефективності різних методів обчислення.

<p align="center">
  <img src="Screenshots/4.PNG" alt="4"/>
</p>
<p align="center">Результати бенчмаркінгу різних методів обчислення на 50,000 ітераціях</p>

## Результати бенчмаркінгу
За результатами тестування на 50,000 ітераціях було отримано наступні показники швидкодії:
- Евклідові відстані: 51.9 мс
- Евклідові просторові: 72.8 мс
- Координати на колі: 10.7 мс
- Об'ємні виміри: 71.4 мс
- Сферичні дуги: 14 мс

## Висновок
В результаті виконання лабораторної роботи було успішно розроблено та протестовано програмне забезпечення для роботи з різними системами координат. Проведене тестування продуктивності виявило суттєві відмінності у швидкодії різних методів обчислення відстаней. Найефективнішим виявився метод координат на колі з часом виконання 10.8 мс, тоді як найповільнішим став метод об'ємних вимірів, що потребував 71.4 мс на виконання. Різниця у швидкодії склала 60.6 мс, що є значущим показником при виконанні великої кількості обчислень та може бути критичним фактором при виборі методу розрахунку в реальних застосуваннях.
