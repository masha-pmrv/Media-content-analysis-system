
## 2. Сценарії  

### 2.1 Сценарій реєстрації нового користувача

**ID**: S1.1  
**НАЗВА**: Реєстрація нового користувача.  
**УЧАСНИКИ**: Система; Користувач.  
**ПЕРЕДУМОВИ**: Відсутні.  
**РЕЗУЛЬТАТ**: Створення нового облікового запису користувача.  
**ВИКЛЮЧНІ СИТУАЦІЇ**: 
1. Користувач прервав процес реєстрації облікового запису.
2. Аккаунт вже створенний.  


**ОСНОВНИЙ СЦЕНАРІЙ**:  
1. Користувач натискає кнопку «Створити новий аккаунт».
2. Користувач заповнює поля: логін, пароль, e-mail.
3. Користувач підтверджує правильність введених даних.
4. Система перевіряє введені дані.
5. Система надсилає підтверження про регестрацію.
6. Користувач підтвержуе регістрацію.
7. Система надає доступ до створеного акаунту.

**ДІАГРАМА**:  

### 2.2 Сценарій авторизації користувача

**ID**: S1.2  
**НАЗВА**: Авторизація користувача.  
**УЧАСНИКИ**: Користувач; Система.   
**ПЕРЕДУМОВИ**: 
1. Наявність облікового запису у користувача.
2. Відсутність обмежень у користування аккаунтом.

**РЕЗУЛЬТАТ**: Успішна авторизація в системі.  
**ВИКЛЮЧНІ СИТУАЦІЇ**:  
1. Користувач ввів некоректні дані.  
2. Користувач перервав процес авторизації.  

**ОСНОВНИЙ СЦЕНАРІЙ**:  
1. Користувач натискає кнопку «Авторизація».  
2. Система пропонує форму авторизації.   
3. Користувач заповнює поля «Логін», «Пароль».  
4. Користувач натискає кнопку «Вхід».  
5. Система авторизує користувача.  

**ДІАГРАМА**:  

### 2.3 Сценарій створення запита користувачем

**ID**: S1.3  
**НАЗВА**: Створення запита користувачем. 
**УЧАСНИКИ**: Користувач; Система.   
**ПЕРЕДУМОВИ**: 
1. Авторизація.
2. Відсутність обмежень у користування аккаунтом.
3. Задання параметрів пошуку.
**РЕЗУЛЬТАТ**: Отримання потрібної інформації.  
**ВИКЛЮЧНІ СИТУАЦІЇ**:  
1. Користувач ввів некоректні дані.  
2. Користувач перервав процес пошуку.
3. Дані відсутні в системі. 

**ОСНОВНИЙ СЦЕНАРІЙ**:  
1. Користувач натискає кнопку "Пошук".
2. Система пропонує форму пошуку.
3. Користувач задає параметри пошуку.
4. Система обробляє задані дані.
5. Система надає інформацію користувачу у заданому форматі.

### 2.4 Сценарій вирішення проблем

**ID**: S1.4  
**НАЗВА**: Вирішення проблем користувачів.
**УЧАСНИКИ**: Користувач; Адмін; Система. 
**ПЕРЕДУМОВИ**: 
1. Авторизація.
2. Відсутність обмежень у користування аккаунтом.
**РЕЗУЛЬТАТ**: Вирішити всю проблему користувача.  
**ВИКЛЮЧНІ СИТУАЦІЇ**:  
1. Користувач задав некоректне питання.  
2. Адміністратор не в змозі вирішити проблему.

**ОСНОВНИЙ СЦЕНАРІЙ**:  
1. Користувач натискає кнопку "Задати питання".
2. Система відкриває діалогове вікно.
3. Система з'єднує користувача та адміністратора.
**ДІАГРАМА**:  

### 2.5 Сценарій стеження за цілісністю та актуальністю інформації в базі даних 

**ID**: S1.5  
**НАЗВА**: Стеження за цілісністю та актуальністю інформації в базі даних. 
**УЧАСНИКИ**: Адмін; Система   
**ПЕРЕДУМОВИ**: 
Відсутні.
**РЕЗУЛЬТАТ**: Залежить від проблеми в системі.  
**ВИКЛЮЧНІ СИТУАЦІЇ**:  
1. Адміністратор не в змозі виправити помилку.
**ОСНОВНИЙ СЦЕНАРІЙ**:  
Все залежить від ситуації.

### 2.6 Сценарій блокування аккаунтів

**ID**: S1.6 
**НАЗВА**: Блокування аккаунтів. 
**УЧАСНИКИ**: Адмін; Користувач; Система.   
**ПЕРЕДУМОВИ**: 
1. Підозрілі дії користувача.
**РЕЗУЛЬТАТ**: 
В залежності від рішення адміністратора:
  1. Блокування аккаунту.
  2. Попередження.
**ВИКЛЮЧНІ СИТУАЦІЇ**:  
1. Система помилилась.

**ОСНОВНИЙ СЦЕНАРІЙ**:  
1. Підозрілі дії користувача.
2. Система сповіщує адміністратора.
3. Адміністратор перевіряє надану інформацію.
4. Адміністратор вибирає одне з можливих варіантів:
  1. Блокування аккаунту;
  2. Попередження;
  
### 2.7 Сценарій сповіщення про помилку

**ID**: S1.3  
**НАЗВА**: Сповіщення про помилку.
**УЧАСНИКИ**: Адмін; Система.   
**ПЕРЕДУМОВИ**: 
1. В роботі системи виникла помилка.
**РЕЗУЛЬТАТ**: Адміністратор дізнається про помилку.  
**ВИКЛЮЧНІ СИТУАЦІЇ**:  
Відсутні.
**ОСНОВНИЙ СЦЕНАРІЙ**:  
1. Система видає помилку.
2. Система сповіщує адміністратора.

### 2.8 Сценарій обробки інформації

**ID**: S1.8  
**НАЗВА**: Обробка інформації.
**УЧАСНИКИ**: Система; Користувач. 
**ПЕРЕДУМОВИ**: 
1. Наявність запиту на обробку інформації.
**РЕЗУЛЬТАТ**: Відфільтрована інформація.
**ВИКЛЮЧНІ СИТУАЦІЇ**:  
1. Дані відсутні в системі.

**ОСНОВНИЙ СЦЕНАРІЙ**:  
1. Система отримує запит.
2. Система відфільтрвує інформацію.
3. Ситема надає результат користувачу.


