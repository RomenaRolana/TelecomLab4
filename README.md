# TelecomLab4
enerateRandomSequence(length): Функція створює випадкову послідовність бітів заданої довжини. Вона проходить через цикл від 0 до зазначеної довжини, генеруючи на кожній ітерації 0 або 1 випадковим чином та додає цей біт до результуючої стрічки.

convolutionalEncode(input, rate, m, polynomial): Функція, що реалізує згорткове кодування. Вона використовує регістр зсуву, який спочатку заповнений нулями, для обчислення кодованих бітів. Розмір регістра зсуву визначається параметром m. Для кожного біту вхідної послідовності функція додає новий біт на початок регістра і видаляє останній, забезпечуючи постійний розмір регістра. За допомогою породжуючих поліномів визначається, які біти з регістра будуть використовуватися для створення кожного вихідного біта.

generateAndDisplaySequences(): Ця функція ініціює процес генерації вхідної послідовності, її кодування та відображення результатів. Вона використовує функцію generateRandomSequence для створення вхідної послідовності довжиною 1000 бітів, потім передає цю послідовність, разом із параметрами швидкості коду, розміру регістра зсуву та породжуючими поліномами, до функції convolutionalEncode для згорткового кодування. Результати відображаються в HTML-елементі з ідентифікатором 'results'.
