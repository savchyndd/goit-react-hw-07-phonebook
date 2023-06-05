# goit-react-hw-06-phonebook

## Критерії приймання

Використовуй цей
[шаблон React-проекту](https://github.com/goitacademy/react-homework-template#readme)
як стартову точку своєї програми.

- Створений репозиторій `goit-react-hw-07-phonebook`.
- Використана бібліотека `Redux Toolkit`.

## Книга контактів

Візьми своє рішення завдання з
[попередньої домашньої роботи](https://github.com/savchyndd/goit-react-hw-06-phonebook.git)
і проведи рефакторинг коду. Видали код, що відповідає за зберігання та читання
контактів з локального сховища, та додай взаємодію з бекендом для зберігання
контактів.

#### Бекенд

Створи свій персональний бекенд для розробки за допомогою UI-сервісу
[mockapi.io](https://mockapi.io/). Зареєструйся використовуючи свій обліковий
запис GitHub. Створи ресурс `contacts` щоб отримати ендпоінт `/contacts`.
Використай конструктор ресурсу та опиши об'єкт контакту як на ілюстрації.

#### Форма стану

Додай у стан Redux обробку індикатора завантаження та помилки. Для цього зміни
форму стану.

```
{
  contacts: {
    items: [],
    isLoading: false,
    error: null
  },
  filter: ""
}
```

#### Операції

Використовуй функцію
[createAsyncThunk](https://redux-toolkit.js.org/api/createAsyncThunk) для
оголошення асинхронних генераторів екшенів та виконання HTTP-запитів. Обробку
екшенів та зміну даних у стані Redux зроби за допомогою
[`createSlice`](https://redux-toolkit.js.org/api/createSlice).

Оголоси наступні операції:

- `fetchContacts` - одержання масиву контактів (метод GET) запитом. Базовий тип
  екшену `"contacts/fetchAll"`.
- `addContact` - додавання контакту (метод POST). Базовий тип екшену
  `"contacts/addContact"`. - `deleteContact` - видалення контакту (метод
  DELETE). Базовий тип екшену `"contacts/deleteContact"`.
