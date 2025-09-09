# API Requests Documentation

## Главная страница

### Посты (лента)

-   `api/v1/posts/?limit=7&offset=0`

### Новости

-   `api/v1/posts/?limit=7&offset=0&content=news`

### Мои посты

-   `api/v1/posts/my/?limit=7&offset=0`

### Дни рождения

-   `api/v1/birthdays/?start_date=2025-09-09&end_date=2025-09-09`
-   `/api/v1/birthdays/birthday-read/?start_date=2025-09-09&end_date=2025-09-09`

---

## Карьера банка

### Лента вакансий

-   `api/v1/posts/?limit=9&offset=0&query=content%3Dvacancy%26`
-   `api/v1/posts/postID`

### Поиск вакансий

-   `api/v1/posts/branches/?`
-   `api/v1/posts/departments/?`
-   `posts/?limit=9&offset=0&query=content%3Dvacancy%26branch%3D23%26department%3D371`

---

## Посты и комментарии

-   `api/v1/posts/postID/comments`
-   `api/v1/comments/`
-   `api/v1/comments/commentID/`

---

## Пользователи (Профиль)

-   `api/v1/users/k_rashidova@cbk.kg/?email=k_rashidova%40cbk.kg`

---

## Реакции

-   `api/v1/reactions/`
-   `api/v1/comments-reactions/`

---

## Поздравления с днем рождения

-   `api/v1/mention/send-notification/`
-   `api/v1/users/mark_birthday_read/`

---

## Мобильная библиотека / Контент

### Категории и жанры

-   `api/v1/library/genre/`
-   `api/v1/library/category/?offset=0&limit=3`
-   `api/v1/library/category/?offset=0&limit=3&genre=<genre>`

### Коллекции и книги

-   `api/v1/library/collection/?limit=5&offset=0`
-   `api/v1/library/book/new-releases/?limit=10&genre=<genre>`
-   `api/v1/library/book/?limit=10&offset=0&genre=<genre>`
-   `api/v1/library/book/?category=<category>&limit=10&offset=0`
-   `api/v1/library/book/topbooks/?limit=10`
-   `api/v1/library/book/bookID/`
-   `api/v1/library/book/382/reservation-status/`
-   `api/v1/library/book/?search=<query>&offset=0&limit=10`

### Breadcrumbs

-   `api/v1/library/breadcrumbs/?genre=<genre>`

### Избранное

-   `api/v1/library/favorite/<bookID>/add/`
-   `api/v1/library/favorite/<bookID>/remove/`

### Предложения книги

-   `/api/v1/library/suggest-book/`

---

> **Примечания**
>
> -   `<genre>` и `<category>` — переменные для выбранного жанра или категории.
> -   `postID`, `commentID`, `bookID` — динамические идентификаторы.
> -   `limit` и `offset` — для пагинации.
