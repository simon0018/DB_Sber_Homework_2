# DB_Sber_Homework_2(MongoDB)
В начале я установил MongoDB Compass

<img width="959" alt="Поставил Mongo" src="https://user-images.githubusercontent.com/89707757/230073148-ee5041a9-fc3f-44b7-8849-957816e481f5.png">

Заполнил базу данных из [этого](https://www.kaggle.com/datasets/shwetabh123/mall-customers) датасета. В базе данных имеется 200 записей про поситетелей магазина 

<img width="761" alt="Заполнил базу данных из датасета" src="https://user-images.githubusercontent.com/89707757/230074049-8593dcea-63d5-462c-a5df-9a3fb9e14eb4.png">


## CRUD-операции 

#### Create
Создал две новых записи с помощью команд ADD DATA -> Insert document
<img width="750" alt="Create" src="https://user-images.githubusercontent.com/89707757/230074077-2fa59a77-b102-480d-b50c-0a23af1439d9.png">

#### Read
Выборка людей младше 30 лет

<img width="758" alt="Read1(Age_lt_30)" src="https://user-images.githubusercontent.com/89707757/230074112-aa5d6b70-df3f-4629-9313-a1a98c095993.png">

Выборка людей с доходом более 132к и менее 16к

<img width="757" alt="Read2" src="https://user-images.githubusercontent.com/89707757/230074158-5a2c4e30-9ed6-4da7-a3f9-a11cb621ed4f.png">

#### Update
Покупатель сменил пол)

<img width="742" alt="Update1" src="https://user-images.githubusercontent.com/89707757/230074200-12c0579d-e2e8-45a0-acfe-5e6975bda807.png">

<img width="746" alt="Update1 1" src="https://user-images.githubusercontent.com/89707757/230074215-13748a8a-a945-491d-86bc-a486840a6d9d.png">
У покупателя изменился доход

<img width="740" alt="Update2" src="https://user-images.githubusercontent.com/89707757/230074239-396e1552-7784-4180-881c-78ddd6d4f12b.png">

<img width="728" alt="Update2 2" src="https://user-images.githubusercontent.com/89707757/230074260-45a86a9b-6284-492f-b2de-c9a92466189e.png">

#### Delete
Удалили первую запись из выборки людей, которым по 34

<img width="753" alt="Delete1" src="https://user-images.githubusercontent.com/89707757/230074289-132b0b78-772d-450c-8e84-2c4cbf83a653.png">

<img width="753" alt="Delete1 1" src="https://user-images.githubusercontent.com/89707757/230074325-a8e95f70-71ba-4547-87bd-d3361e5a02e0.png">

## Создание индекса + сравнение производительности запросов
Переходим в окно MONGOSH

Делаем выборку по полу
<img width="492" alt="выборка 1" src="https://user-images.githubusercontent.com/89707757/230081696-eea24fd9-db1b-4387-bd6a-5ea0eaaf120c.png">

Считаем производительность

<img width="512" alt="производительность 1" src="https://user-images.githubusercontent.com/89707757/230081715-00a35819-301d-4e80-b327-34c65de79d84.png">

Создаем индекс

<img width="299" alt="Создание индекса" src="https://user-images.githubusercontent.com/89707757/230081675-30b35839-27ea-4e08-9e34-cf66ae1e6d8e.png">

Считаем производительность по той же выборке и убеждаемся, что результат стал в разы лучше

<img width="533" alt="производительность 2" src="https://user-images.githubusercontent.com/89707757/230081732-eb866276-77a1-45f3-a693-37bf2e5e6a1f.png">
