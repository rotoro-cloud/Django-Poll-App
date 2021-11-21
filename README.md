# Django-Poll-App

Приложение Django poll - это полнофункциональное приложение для опросов. Вы должны зарегистрироваться в этом приложении, чтобы смотреть опросы и голосовать. Если вы уже проголосовали, то вы не можете проголосовать снова. Только владелец опроса может редактировать, обновлять, удалять опрос, удалять данные из голосования и завершать опрос. Если опрос завершен, в нем нельзя голосовать. Завершенный опрос показывает пользователю только окончательный результат. Есть возможность поиска по опросам. Также пользователь может фильтровать опросы по имени, дате публикации и количеству проголосовавших. Пагинация будет работать даже после применения фильтра.

<h1>Как начать</h1>
<p>Эти инструкции позволят вам запустить копию проекта на вашем локальном компьютере в целях разработки и тестирования.</p>

<h2>Предварительные требования</h2>

`python >= 3.5, django>=2.0`

<h2>Установка</h2>
Склонируй репозиторий

```
git clone https://github.com/rotoro-cloud/Django-Poll-App.git
```

Установи зависимости python

```
pip install -r requirements.txt
```

Установи утилиты работы с БД

```
pip install mysqlclient
```

<h2>Настройка</h2>
Приложение настроено на работу с MySQL. База уже установлена. Настройки находятся в файле `pollme/settings.py`. Тебе нужно добавить их в локальную MySQL

```
sudo vi lets_quiz/settings.py
```

Добавь нужные данные

```
[client] 
database = lets_quiz  
user = djangouser  
password = PASSWORD  
default-character-set = utf8
```

Перезапусти MySQL
```
sudo systemctl daemon-reload
sudo systemctl restart mysql
```

Создай структуру БД
```
python3 manage.py migrate
```

Создай пользователя для администрирования
```
python3 manage.py createsuperuser
```

<h2>Запуск</h2>
Приложение запускается на 8000 порту
```
python3 manage.py runserver 0.0.0.0:8000
```

<p>Приложение будет доступно http://YOUR-IP:8000 твоего браузера</p>

<h2>Project snapshot</h2>
<h3>Home page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409444-0e40a600-1b8c-11e9-9ab0-27d759db8973.jpg" width="100%"</img> 
</div>

<h3>Login Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409509-36c8a000-1b8c-11e9-845a-65b49262aa53.png" width="100%"</img> 
</div>

<h3>Registration Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409562-5cee4000-1b8c-11e9-82f6-1aa2df159528.png" width="100%"</img> 
</div>

<h3>Poll List Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409728-d423d400-1b8c-11e9-8903-4c08ba64512e.png" width="100%"</img> 
</div>

<h3>Poll Add Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409796-fe759180-1b8c-11e9-941b-c1202956cca4.png" width="100%"</img> 
</div>

<h3>Polling page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409843-1e0cba00-1b8d-11e9-9109-cceb79a6a623.png" width="100%"</img> 
</div>

<h3>Poll Result Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409932-60ce9200-1b8d-11e9-9c83-c59ba498ca8b.png" width="100%"</img> 
</div>

<h3>Poll Edit Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51410008-92dff400-1b8d-11e9-8172-c228e4b60e28.png" width="100%"</img> 
</div>

<h3>Choice Update Delete Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51410442-dc7d0e80-1b8e-11e9-8f8e-18e6d7bb70fb.png" width="100%"</img> 
</div>

<h2>Author</h2>
<blockquote>
  Mahmudul alam<br>
  Email: expelmahmud@gmail.com
</blockquote>

<div align="center">
    <h3>========Thank You !!!=========</h3>
</div>
