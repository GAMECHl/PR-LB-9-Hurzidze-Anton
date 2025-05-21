# PR-LB-9-Hurzidze-Anton
## Хурцидзе Антон IПЗ 3.02 Практична-Лабораторна робота № 9

## Тема: Неперервна доставка
## Мета: ознайомитися з принципами і практиками неперервної доставки, сформувати навички роботи з хмарними сервісами Azure
#### 1. Заходимо на сторіку https://portal.azure.com/#home та використовуючи пошук переходимо на сторінку ``App Services``, натискаємо кнопку ``Create`` та обираємо ``Web App``:
![1](https://github.com/GAMECHl/PR-LB-9-Hurzidze-Anton/blob/main/1.png)
#### Рис. 1 - Створення веб-застосунку

#### 2. Заповнюємо поля наступним чином та натискаємо на кнопку ``Rewiew+Create``:
![2](https://github.com/GAMECHl/PR-LB-9-Hurzidze-Anton/blob/main/2.png)
![3](https://github.com/GAMECHl/PR-LB-9-Hurzidze-Anton/blob/main/3.png)
#### Рис. 2 - Заповнені поля

#### 3. Для створення ``Azure Service principal`` потрібно відкрити командний рядок, який розташовується справа від пошуку:
![4](https://github.com/GAMECHl/PR-LB-9-Hurzidze-Anton/blob/main/4.png)
#### Рис. 3 - Командний рядок

#### 4. Далі вводимо наступну команду замінивши всі рядки як цей: <line>, на нашу інформацію з створенного застосунку: "az ad sp create-for-rbac --name "myApp" --role contributor --scopes /subscriptions/<subscription_id>/resourceGroups/<resource_group_name> --json-auth".
![5](https://github.com/GAMECHl/PR-LB-9-Hurzidze-Anton/blob/main/5.png)
#### Рис. 4 - Команда з моєю інформацією

#### 5. Після корректного запуску команди ми отримаємо секретну інформацію про наш проект і про наш аккаунт:
![6](https://github.com/GAMECHl/PR-LB-9-Hurzidze-Anton/blob/main/6.png)
#### Рис. 5 - Секретна інформація

#### 6. Потім переходимо в гітхаб репозіторій із минулої лабороторної та переходимо по наступним сторінкам: ``settings >>> secrets and variables > actions``, та натискаємо ``New Repository Secret`` та вводимо інформацію яку ми добули в минулому пункті наступним чином:
![7](https://github.com/GAMECHl/PR-LB-9-Hurzidze-Anton/blob/main/7.png)
#### Рис. 6 - Створення нового секрету

#### 7. Переходимо до воркфлоу який ми створили в минулому і редактуємо його наступним чином:
![8](https://github.com/GAMECHl/PR-LB-9-Hurzidze-Anton/blob/main/8.png)
#### Рис. 7 - Файл docker-build.yml

#### 8. Після підтвердження змін перейдемо до сторінки ``Actions`` та дивимся на стан деплоя:
![9](https://github.com/GAMECHl/PR-LB-9-Hurzidze-Anton/blob/main/9.png)
#### Рис. 8 - Успішний деплой

#### 9. І нарешті переходимо за настуним посиланням https://pr-lb-9-dfa9e8hjbrcqceh5.westeurope-01.azurewebsites.net/(воно розташовується в деплої в вкладці Deploy to Azure Web App) та дивимся на сторінку:
![10](https://github.com/GAMECHl/PR-LB-9-Hurzidze-Anton/blob/main/10.png)
#### Рис. 9 - Привітальна сторінка проекту

## Висновки: У ході виконання лабораторно-практичної роботи я ознайомився з принципами і практиками неперервної доставки та сформував навички роботи з хмарними сервісами Azure
