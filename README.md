**GIT Homework 1

Для выполнения задания у вас должен быть установлен для Windows - Git Bash. Создан аккаунт в GitHub. Все шаги сценария выполняйте в терминале Git Bash, Terminal, в папке под гитом.

Как отправить ДЗ на проверку.
 1. Создайте текстовый файл, как в первом ДЗ по Terminal.
 2. Сценарий перенесите в этот файл.
 3. Напротив каждого действия - напишите команду в Git Bash
Файл со сценарием и ссылку на свой гит хаб.

**JSON
4. Создать внешний репозиторий c названием JSON. На сайте GitHub

5. Клонировать репозиторий JSON на локальный компьютер - git clone #вставляем сюда скопированную ссылку из  <>Code по протоколу https)

6. Внутри локального JSON создать файл “new.json”.
**cat > new.json

7. Добавить файл под гит.
**git add new.json

8. Закоммитить файл.
**git commit -m “comments”

 9. Отправить файл на внешний GitHub репозиторий.
**git push

 10. Отредактировать содержимое файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
**nano new.json
{
	"name": "Natalia",
	"lastName": "Tokareva",
	"quantityPet": 1,
	"salaryExpected": "500 USD"
}

 11. Отправить изменения на внешний репозиторий - git commit -a -m “new.json” && git push

 12. Создать файл preferences.json
cat > preferences.json

 13. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
nano preferences.json
{
	"favoriteFilm": "Sea Inside",
	"favoriteSeries": "Friends",
	"favoriteFood": ["Khinkali", "Pho Bo", "soup", "pasta"],
	"favoriteSeason": ["spring", "summer"],
	"Country": "the USA"
}
Ctrl+O, Ctrl+X

 14. Создать файл skills.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
cat > skills.json
{
"Skills": [
"API через Postman", "сниффинг http web трафика через Charles и Fiddler", "Dev Tools веб браузеров, командная строка", "основы SQL техники тест-дизайна"
]
}

 15. Отправить сразу 2 файла на внешний репозиторий
git add ./

 16. На веб интерфейсе создать файл bug_report.json
 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
{
	"id": "BR-1",
	"Summary": "Кнопка Отправить не реагирует на клик на странице оформления заказа.",
	"Project": "www.test.pitomets.com",
	"Version": "5.1",
	"Severity": "Critical",
	"Priority": "Middle",
	"Status": "Open",
	"Author": "Tokareva Natalia",
	"Assigned To": "Lead Developer",
	"Description": {
		"Precondition": {
			"1": "Зайти на сайт www.test.pitomets.com",
			"2": "Перейти на страницу Питомцы"
		},
		"Environment": "Windows 11 Pro, Google Chrome v: 94.0.4606.71 (x86_64)",
		"Steps to reproduce": {
			"1": "Кликнуть на кнопку Оформить заказ в карточке питомца",
			"2": "Заполнить поле Имя",
			"3": "Заполнить поле телефон",
			"4": "Заполнить поле E-mail",
			"5": "Нажать кнопку Отправить"
		},
		"Actual result": "Кнопка “Отправить” в форме заказа питомца не реагирует на клик.",
		"Expected result": "Пользователь перенаправляется на страницу подтверждения заказа. Есть сообщение, что заказ №#### отправлен, менеджер с вами свяжется в ближайшее время"
	},
	"Attachment": "https://drive.google.com/..."
}

 19. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 20. Синхронизировать внешний и локальный репозиторий JSON
git pull
