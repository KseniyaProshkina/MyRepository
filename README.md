# MyRepository
## Запуск postman-коллекции:
__Шаги:__
1. Изучила [документацию к API GitHub Issues](https://docs.github.com/en/rest/issues/issues?apiVersion=2022-11-28#about-issues)
2. На GitHub создала токен личного доступа в разделе Developer Settings > Personal access tokens
3. Создала коллекцию в Postman нажатием с названием "Аттестация. GitHub issues"
4. Настроила авторизацию в разделе Authotization:
   * тип: Bearer Token
5. Создала переменную в разделе Variables
   * Variable: MyToken 
7. Создала первый запрос на добавление проблемы (issues):
   * Authotization
   * метод: POST
   * url: https://api.github.com/repos/KseniyaProshkina/MyRepository/issues
   * 
   
