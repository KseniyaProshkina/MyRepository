# MyRepository
## Запуск postman-коллекции:
__Шаги:__
1. Изучила [документацию к API GitHub Issues](https://docs.github.com/en/rest/issues/issues?apiVersion=2022-11-28#about-issues)
2. На GitHub создала токен личного доступа в разделе Developer Settings > Personal access tokens
3. Создала коллекцию в Postman с названием "Аттестация. GitHub issues"
4. Настроила авторизацию в разделе Authotization:
   * тип: Bearer Token
5. Создала переменную для токена в разделе Variables
   * Variable: **MyToken**
6. Создала запрос на добавление проблемы Issue 1 методом POST на URL https://api.github.com/repos/KseniyaProshkina/MyRepository/issues
8. В данном запросе создала переменную https://api.github.com > **BaseURL**
9. В данном запросе в разделе Tests с помощью скрипта создала автоматизированную переменную **i_number** для параметра *"number"*, который идентифицирует проблему
10. В данном запросе в разделе Tests добавила проверку "Status code is 200" на статус код ответа 201
11. Создала запрос на получение списка проблем методом GET на URL {{**BaseURL**}}/repos/KseniyaProshkina/MyRepository/issues
12. В данном запросе в разделе Tests добавила проверку "Status code is 200" на статус код ответа 200 
13. Создала запрос на редактирование названия проблемы на Issue 2 методом PATCH на URL {{**BaseUrl**}}/repos/KseniyaProshkina/MyRepository/issues/{{**i_number**}}
14. В данном запросе в разделе Tests добавила проверку "Status code is 200" на статус код ответа 200 
15. Создала запрос на редактирование состояния проблемы - закрытая методом PATCH на URL {{**BaseUrl**}}/repos/KseniyaProshkina/MyRepository/issues/{{**i_number**}}
16. В данном запросе в разделе Tests добавила проверку "Status code is 200" на статус код ответа 200 
17. Создала запрос на удаление проблемы методом DELETE на URL {{BaseUrl}}/repos/KseniyaProshkina/MyRepository/issues/{{i_number}}/lock
18. В данном запросе в разделе Tests добавила проверку "Status code is 200" на статус код ответа 204
    
   
