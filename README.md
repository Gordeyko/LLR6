# Лабораторная работа №6
 

Порядок выполнения работы:
1. Создала аккаунт на сайте GitHub.
2. Сделала копию в личное хранилище из https://github.com/Kurtyanik/LR6/ (Fork).
3. Установила Git 
4. После установки настроила клиент git, введя имя пользователя (Группа
Фамилия И.О.) и email.

```
git config --global user.name "В3441 Гордейко Алена Леонидовна"

git config --global user.email "LunarGames31@bk.ru"
```

![image](https://github.com/user-attachments/assets/81f61744-2f55-4b73-983f-a492601320d4)


6. Клонировала свой личный удалённый репозиторий на компьютер (назвала работу LLR6, так как переделывала 3 раза)
   
```
git clone https://github.com/Gordeyko/LLR6

```

![image](https://github.com/user-attachments/assets/3fe38a49-d9b4-457d-b39d-98c09ece39a4)


7. Добавила файл через интерфейс GitHub. Подтянула изменения в
локальный репозиторий. Работу продолжила локально, перейдя в папку
   
```
cd LLR6
```

![image](https://github.com/user-attachments/assets/da438b65-9488-41b8-a96e-5243a67e706a)


```
git pull

```

![image](https://github.com/user-attachments/assets/8b5e1bcc-f187-4eef-a351-8c457f9e8fbd)



8. Получила историю операций для каждой из веток.
    
```
git log --oneline
```

![image](https://github.com/user-attachments/assets/2056a539-70a5-48db-b297-ac16f60713f7)


9. Просмотрела последние изменения.
    
```
git log -p 
```

![image](https://github.com/user-attachments/assets/e5d60de1-03ca-45d1-8d8c-a8d0221d3c69)


10. Cоздала новую ветку, внесла изменения и выполнила слияние в ветку master
    
```
git checkout -b branch1
git add .
git commit -m "изменение1"
git checkout master
git merge branch1
```

![image](https://github.com/user-attachments/assets/c8b9c795-42f2-410e-af2a-89ae665e4cf8)

![image](https://github.com/user-attachments/assets/d583fb5f-7690-4ce1-b41a-0b1b28b17910)


11. Удалила побочную ветку после успешного слияния (не сохранился скрин)
    
```
git branch -d branch1
```

![image](https://github.com/user-attachments/assets/bf8c8c1a-7404-46bd-8f40-607ec09c04bb)


12. Сделала 2 изменения и зафиксировала их
    
```
git add .
git commit -m "изменение2"
git add .
git commit -m "изменение3"
```
![image](https://github.com/user-attachments/assets/76e6ff70-c0af-4ea2-8196-e06de83b3315)


![image](https://github.com/user-attachments/assets/ac9978f2-98ee-4231-8eb2-954c3472d3e2)


13. Сделала откат коммита
    
```
git log --oneline
git revert 5351a1d
```

![image](https://github.com/user-attachments/assets/462c0927-e39a-4a8d-baec-8f4bbe57a499)

![image](https://github.com/user-attachments/assets/d88022f9-c438-41bc-a425-a3858661daf7)



14. Создала ветку для отчёта
```
git checkout -b othet
```

![image](https://github.com/user-attachments/assets/97658f9e-7925-4520-96f0-d903e90f0e13)


15. Оформила отчёт в файле README.md, используя markdown синтаксис. Файлы снимков экрана разместила в отдельной папке screen

16. Получила историю операций в форматированном виде
    
```
git log --pretty=format:"%h %ad | %s%d [%an]" --date=short
```

![image](https://github.com/user-attachments/assets/05583214-7d47-4468-a6ec-d68ed15e9da8)


17. Отправила локальные изменения в сетевое хранилище GitHub
    
```
git push origin otchet
```

![image](https://github.com/user-attachments/assets/a058162c-8714-43f9-ade1-d98dbb8e958e)

