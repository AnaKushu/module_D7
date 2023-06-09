Проект "Новостной портал".
Сайт представляет собой оформленный Bootstrap-шаблон со встроенными пользовательскими данными.
В ходе реализации проекта были созданы модели:
1. Модель Author: модель, содержащая объекты всех авторов.
2. Модель Category: Категории новостей/статей — темы, которые они отражают. На данном сайте отражены 4 раздела: Наука, Техника, Технология и Информационные технологии. Категории реализованы с возможностью пользователей подписаться (или отписаться) на любую из них и получать рассылку при создании новой новости или статьи.
3. Модель Post: модель содержит в себе статьи и новости, которые создают авторы.
4. Модель PostCategory: промежуточная модель для связи «многие ко многим»: связь «один ко многим» с моделью Post; связь «один ко многим» с моделью Category.
5. Модель Comment: под каждой новостью/статьёй можно оставлять комментарии, поэтому таким образом организован их способ хранения.

Все статьи в виде кликабельных заголовков, даты написания, кликабельных категорий и краткого описания (первые 25 символов статьи) представлены на странице с адресом /news/. Новости выводятся в порядке от более свежей к самой старой.
В некоторых статьях присутствуют слова, которые следовало цензурировать. Для выполнения данной задачи написан собственный фильтр censor, который заменяет буквы нежелательных слов в заголовках и текстах статей на символ «*».
На отдельной странице Search реализована возможность искать новости по определённым критериям: -название; -категория; -поиск позже указываемой даты создания статьи/новости.
Для администратора сайта и пользователей группы Авторы реализована возможность создания, редактирования и удаления статьи/новости.
На сайте есть возможность регистрации с помощью почты и пароля или через Yandex-аккаунт с верификацией почты. 
На данном этапе работы над проектом реализована возможность отправки списка новых статей на почту подписчиков категорий каждую неделю.
