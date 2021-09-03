# Проект YaMDb
## бэкенд проекта и API для него

Проект YaMDb собирает отзывы пользователей на произведения. Произведения делятся на категории: «Книги», «Фильмы», «Музыка». Список категорий может быть расширен администратором (например, можно добавить категорию «Изобразительное искусство» или «Ювелирка»).
Сами произведения в YaMDb не хранятся, здесь нельзя посмотреть фильм или послушать музыку.
В каждой категории есть произведения: книги, фильмы или музыка. Например, в категории «Книги» могут быть произведения «Винни-Пух и все-все-все» и «Марсианские хроники», а в категории «Музыка» — песня «Давеча» группы «Насекомые» и вторая сюита Баха.
Произведению может быть присвоен жанр из списка предустановленных (например, «Сказка», «Рок» или «Артхаус»). Новые жанры может создавать только администратор.
Благодарные или возмущённые пользователи оставляют к произведениям текстовые отзывы и ставят произведению оценку в диапазоне от одного до десяти; из пользовательских оценок формируется усреднённая оценка произведения — рейтинг. На одно произведение пользователь может оставить только один отзыв.

### Как запустить проект:

Клонировать репозиторий:

```
git clone https://github.com/Andrey-A-K/infra_sp2
```

Перейти в него в командной строке:

```
cd infra_sp2
```

Запустить проект(при первом запуске начнется сборка):

```
docker-compose up

```

### Для работы в админке создайте суперюзера:

```
sudo docker exec -it <id_вашего_контейнера> bash
```

```
python manage.py createsuperuser
```

И залогиньтесь по адресу:

```
http://127.0.0.1/admin/
```



### документация к API доступна по адресу:

```
http://127.0.0.1/redoc/
```
