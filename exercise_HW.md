Postman. HW_1

Создать запросы в Postman.

Protocol: http IP: 162.55.220.72 Port: 5005

EP_1 Method: GET EndPoint: /get_method request url params: name: str age: int

response: [ “Str”, “Str” ]

==================

EP_2 Method: POST EndPoint: /user_info_3 request form data: name: str age: int salary: int

response: {'name': name, 'age': age, 'salary': salary, 'family': {'children': [['Alex', 24], ['Kate', 12]], 'u_salary_1_5_year': salary * 4}}

==================

EP_3 Method: GET EndPoint: /object_info_1 request url params: name: str age: int weight: int

response: {'name': name, 'age': age, 'daily_food': weight * 0.012, 'daily_sleep': weight * 2.5}

==================

EP_4 Method: GET EndPoint: /object_info_2 request url params: name: str age: int salary: int

response: {'start_qa_salary': salary, 'qa_salary_after_6_months': salary * 2, 'qa_salary_after_12_months': salary * 2.7, 'qa_salary_after_1.5_year': salary * 3.3, 'qa_salary_after_3.5_years': salary * 3.8, 'person': {'u_name': [user_name, salary, age], 'u_age': age, 'u_salary_5_years': salary * 4.2} }

==================

EP_5 Method: GET EndPoint: /object_info_3 request url params: name: str age: int salary: int

response: {'name': name, 'age': age, 'salary': salary, 'family': {'children': [['Alex', 24], ['Kate', 12]], 'pets': {'cat':{'name':'Sunny', 'age': 3}, 'dog':{'name':'Luky', 'age': 4}}, 'u_salary_1_5_year': salary * 4} }

==================

EP_6 Method: GET EndPoint: /object_info_4 request url params: name: str age: int salary: int

response: {'name': name, 'age': int(age), 'salary': [salary, str(salary * 2), str(salary * 3)]}

==================

EP_7 Method: POST EndPoint: /user_info_2 request form data: name: str age: int salary: int

response: {'start_qa_salary': salary, 'qa_salary_after_6_months': salary * 2, 'qa_salary_after_12_months': salary * 2.7, 'qa_salary_after_1.5_year': salary * 3.3, 'qa_salary_after_3.5_years': salary * 3.8, 'person': {'u_name': [user_name, salary, age], 'u_age': age, 'u_salary_5_years': salary * 4.2} }

      32_channel, [02.01.2023 22:14]
HW_2 Postman

http://162.55.220.72:5005/first

Отправить запрос.
Статус код 200
Проверить, что в body приходит правильный string.
http://162.55.220.72:5005/user_info_3

Отправить запрос.
Статус код 200
Спарсить response body в json.
Проверить, что name в ответе равно name s request (name вбить руками.)
Проверить, что age в ответе равно age s request (age вбить руками.)
Проверить, что salary в ответе равно salary s request (salary вбить руками.)
Спарсить request.
Проверить, что name в ответе равно name s request (name забрать из request.)
Проверить, что age в ответе равно age s request (age забрать из request.)
Проверить, что salary в ответе равно salary s request (salary забрать из request.)
Вывести в консоль параметр family из response.
Проверить что u_salary_1_5_year в ответе равно salary*4 (salary забрать из request)
http://162.55.220.72:5005/object_info_3

Отправить запрос.
Статус код 200
Спарсить response body в json.
Спарсить request.
Проверить, что name в ответе равно name s request (name забрать из request.)
Проверить, что age в ответе равно age s request (age забрать из request.)
Проверить, что salary в ответе равно salary s request (salary забрать из request.)
Вывести в консоль параметр family из response.
Проверить, что у параметра dog есть параметры name.
Проверить, что у параметра dog есть параметры age.
Проверить, что параметр name имеет значение Luky.
Проверить, что параметр age имеет значение 4.
http://162.55.220.72:5005/object_info_4

Отправить запрос.
Статус код 200
Спарсить response body в json.
Спарсить request.
Проверить, что name в ответе равно name s request (name забрать из request.)
Проверить, что age в ответе равно age из request (age забрать из request.)
Вывести в консоль параметр salary из request.
Вывести в консоль параметр salary из response.
Вывести в консоль 0-й элемент параметра salary из response.
Вывести в консоль 1-й элемент параметра salary параметр salary из response.
Вывести в консоль 2-й элемент параметра salary параметр salary из response.
Проверить, что 0-й элемент параметра salary равен salary из request (salary забрать из request.)
Проверить, что 1-й элемент параметра salary равен salary*2 из request (salary забрать из request.)
Проверить, что 2-й элемент параметра salary равен salary*3 из request (salary забрать из request.)
Создать в окружении переменную name
Создать в окружении переменную age
Создать в окружении переменную salary
Передать в окружение переменную name
Передать в окружение переменную age
Передать в окружение переменную salary
Написать цикл который выведет в консоль по порядку элементы списка из параметра salary.
http://162.55.220.72:5005/user_info_2

Вставить параметр salary из окружения в request
Вставить параметр age из окружения в age
Вставить параметр name из окружения в name
Отправить запрос.
Статус код 200
Спарсить response body в json.
Спарсить request.
Проверить, что json response имеет параметр start_qa_salary
Проверить, что json response имеет параметр qa_salary_after_6_months
Проверить, что json response имеет параметр qa_salary_after_12_months
Проверить, что json response имеет параметр qa_salary_after_1.5_year
Проверить, что json response имеет параметр qa_salary_after_3.5_years
Проверить, что json response имеет параметр person
Проверить, что параметр start_qa_salary равен salary из request (salary забрать из request.)
Проверить, что параметр qa_salary_after_6_months равен salary*2 из request (salary забрать из request.)
Проверить, что параметр qa_salary_after_12_months равен salary*2.7 из request (salary забрать из request.)
Проверить, что параметр qa_salary_after_1.5_year равен salary*3.3 из request (salary забрать из request.)
Проверить, что параметр qa_salary_after_3.5_years равен salary*3.8 из request (salary забрать из request.)
Проверить, что в параметре person, 1-й элемент из u_name равен salary из request (salary забрать из request.)
Проверить, что что параметр u_age равен age из request (age забрать из request.)
Проверить, что параметр u_salary_5_years равен salary*4.2 из request (salary забрать из request.)
***Написать цикл который выведет в консоль по порядку элементы списка из параметра person.
