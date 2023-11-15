# Лабараторная работа 6
## Цель работы:
Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.
## Ход работы:
1. Аккаунт GitHub был создан до выполнения лабораторной работы https://github.com/X-mite
2. Сделана копия (Fork)
   
    ![1](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/1.png)
   
3. Git был установлен ранее
4. Настройка клиента git

    Изменено имя пользователя.
    ```sh
    git config --global user.name "4216 Ефремов М. Д."
    ```
    ![2](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/2.png)
    
    Изменен email.
    ```sh
    git config --global user.email "maxefremov04092004@gmail.com"
    ```
    
    ![3](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/3.png)
    
5. Клонирование репозитория
    ```sh
    git clone https://github.com/CALAMBIK/LR6.git
    ```
    
    ![4](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/4.png)
    
    ![5](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/5.png)
    
6. Добавлен файл через GitHub, подтянуты изменения в локальный репозиторий
    Добавлен файл через GitHub.

    ![6](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/6.png)
    
    Подтянуты изменения в локальный репозиторий.
    ```sh
    git pull
    ```
    
    ![7](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/7.png)
    
7. История операций для каждой из веток
    Для master
    ```sh
    git log
    ```
    
    ![8](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/8.png)
    
    Для branch1
    ```sh
    git log origin/branch1
    ```
    
    ![9](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/9.png)
    
8. Последние изменения
    ```sh
    git status
    ```
    
    ![10](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/10.png)
    
9. Выполнено слияние в ветку master, конфликт решен
    Слияние веток.
    ```sh
    git merge branch1
    ```
    
    ![11](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/11.png)
    
    Зафиксированы изменения.
    ```sh
    git add mergefile.txt
    git commit -m"conflict resolution"
    ```
    
10. Удалена побочная ветка после успешного слияния
    
    При слиянии ветка удалилась автоматически.

    ![12](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/12.png)
    
    Удаление ветки на GitHub
    ```sh
    git push origin -d branch1
    ```
    
    ![13](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/13.png)
    
11. Изменения сделаны и зафиксированы
12. Сделан откат коммита
    
    ```sh
    git reset --hard HEAD~
    ```
    
13. Создана ветка для отчета

    ![15](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/15.png)

14. Получена история операций в форматированном виде
    
    ![16](https://github.com/X-mite/LR6/blob/otchet/%D0%9E%D0%9F2/16.png)

