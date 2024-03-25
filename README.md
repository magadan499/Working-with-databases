Проект по базе данных
Проект позволяет получить данные о компаниях и вакансиях с сайта hh.ru, спроектировать таблицы в БД PostgreSQL и загрузить полученные данные в созданные таблицы.

Для работы с проектом необходимо
Создать файл с названием database.ini, который заполняется следующим образом: [postgresql] host=YourHost user=YourUser password=YourPassword port=YourPort

Работа программы:
При запуске файла main будут получены по 20 актуальных вакансий от 10 самых востребованных IT компаний с сайта HeadHunter.ru Далее в PostgreSQL создается база данных с названием 'headhunter' и таблицами 'employers' и 'vacancies'. После этого запустится работа с пользователем, которая предложит посмотреть несколько выводов по следующим методам:

get_companies_and_vacancies_count(): получает список всех компаний и количество вакансий у каждой компании.
get_all_vacancies(): получает список всех вакансий с указанием названия компании, названия вакансии и зарплаты и ссылки на вакансию.
get_avg_salary(): получает среднюю зарплату по вакансиям.
get_vacancies_with_higher_salary(): получает список всех вакансий, у которых зарплата выше средней по всем вакансиям.
get_vacancies_with_keyword(): получает список всех вакансий, в названии которых содержатся переданные в метод слова, например “python”.