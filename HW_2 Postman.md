HW_2 Postman

http://162.55.220.72:5005/first	
1. Отправить запрос.

![image](https://user-images.githubusercontent.com/83454778/168448935-436435e1-bb79-4f38-97da-fce0d91401ae.png?raw=true)  
2. Статус код 200

![image](https://user-images.githubusercontent.com/83454778/168448986-d45149ce-4c0a-4bea-8232-c913ba650a58.png?raw=true)  
3. Проверить, что в body приходит правильный string.

![image](https://user-images.githubusercontent.com/83454778/168448997-6620eaa5-7bed-47ed-b687-3d19d1a4bcaf.png?raw=true)

http://162.55.220.72:5005/user_info_3
1. Отправить запрос.

![image](https://user-images.githubusercontent.com/83454778/168449112-fb8511ff-8848-40f8-850a-b0282f197bd6.png?raw=true)

2. Статус код 200

![image](https://user-images.githubusercontent.com/83454778/168449120-7f1d7cc8-13d5-4953-b8c7-01193842099a.png?raw=true)

3. Спарсить response body в json

      let jsonData = pm.response.json();

4. Проверить, что name в ответе равно name s request (name вбить руками.)

![image](https://user-images.githubusercontent.com/83454778/168449370-28893e77-5b47-4664-9ca7-d6e314b53159.png?raw=true)

5. Проверить, что age в ответе равно age s request (age вбить руками.)

![image](https://user-images.githubusercontent.com/83454778/168449411-9cc98268-0179-4613-8889-1b4187ae4be2.png?raw=true)

6. Проверить, что salary в ответе равно salary s request (salary вбить руками.)

![image](https://user-images.githubusercontent.com/83454778/168449432-359ab7d0-93be-4d9a-ad13-04e30cee1bee.png?raw=true)

7. Спарсить request.

      let  req = request.data

8. Проверить, что name в ответе равно name s request (name забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168449574-6f0d622d-bf47-46df-8125-79c47a356764.png?raw=true)

9. Проверить, что age в ответе равно age s request (age забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168449607-ea7caf91-f8b0-4e44-a807-b283e2a5cf98.png?raw=true)

10. Проверить, что salary в ответе равно salary s request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168449684-8abc8d4e-ab03-4d7f-923f-f52b7e3aaf7c.png?raw=true)

11. Вывести в консоль параметр family из response.

      console.log(jsonData.family)

12. Проверить что u_salary_1_5_year в ответе равно salary*4 (salary забрать из request)

![image](https://user-images.githubusercontent.com/83454778/168449770-435bd6d7-b65a-4bc8-a8a5-a2e9b83176ae.png?raw=true)

http://162.55.220.72:5005/object_info_3
1. Отправить запрос.

![image](https://user-images.githubusercontent.com/83454778/168449816-b967fb5f-1036-4095-a488-80e43b902b00.png?raw=true)

2. Статус код 200

![image](https://user-images.githubusercontent.com/83454778/168449823-7d2947fd-d2ea-43b3-af66-93dee4c305dc.png?raw=true)

3. Спарсить response body в json.

      let jsonData = pm.response.json();

4. Спарсить request.

      let query = {};
      pm.request.url.query.all().forEach((param) => { query[param.key] = param.value});

5. Проверить, что name в ответе равно name s request (name забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168450379-39ce8d19-746a-4f63-bbeb-2846aae73c74.png?raw=true)

6. Проверить, что age в ответе равно age s request (age забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168450400-11c68ca9-009d-4829-8f1a-f8b8d0c0daa4.png?raw=true)

7. Проверить, что salary в ответе равно salary s request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168450424-d7328149-683d-45b9-a126-60e73f8cfb08.png?raw=true)

8. Вывести в консоль параметр family из response.

      console.log(jsonData.family)

9. Проверить, что у параметра dog есть параметры name.

![image](https://user-images.githubusercontent.com/83454778/168450661-51a4dded-89c8-4d62-80d4-b4b30690bb73.png?raw=true)

10. Проверить, что у параметра dog есть параметры age.

![image](https://user-images.githubusercontent.com/83454778/168450685-12f61605-361a-4471-a036-50f883ac9794.png?raw=true)

11. Проверить, что параметр name имеет значение Luky.

![image](https://user-images.githubusercontent.com/83454778/168450697-31e728b0-26fb-4a53-9e5f-4d0592225819.png?raw=true)

12. Проверить, что параметр age имеет значение 4.

![image](https://user-images.githubusercontent.com/83454778/168450724-30fcb4d0-cb94-4595-8e23-522ac7ec4d61.png?raw=true)

http://162.55.220.72:5005/object_info_4
1. Отправить запрос.

![image](https://user-images.githubusercontent.com/83454778/168450818-2b251561-177f-4e68-9aaf-efabf2c60032.png)

2. Статус код 200

![image](https://user-images.githubusercontent.com/83454778/168450782-8e71f8ab-03ee-4d64-a16b-03852c606bed.png)

3. Спарсить response body в json.

      let jsonData = pm.response.json();

4. Спарсить request.

      let query = {};
      pm.request.url.query.all().forEach((param) => { query[param.key] = param.value});

5. Проверить, что name в ответе равно name s request (name забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168450845-209578ab-48ef-4342-ac93-ff30520cc2e2.png)

6. Проверить, что age в ответе равно age из request (age забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168450873-f570ed8e-12a9-40e8-a48a-3b1aa6ba3e16.png)

7. Вывести в консоль параметр salary из request.

      console.log(query.salary)

8. Вывести в консоль параметр salary из response.

      console.log(jsonData.salary)

9. Вывести в консоль 0-й элемент параметра salary из response.

      console.log(jsonData.salary[0])
      
10. Вывести в консоль 1-й элемент параметра salary параметр salary из response.

      console.log(jsonData.salary[1])

11. Вывести в консоль 2-й элемент параметра salary параметр salary из response.

      console.log(jsonData.salary[2])

12. Проверить, что 0-й элемент параметра salary равен salary из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451057-0ed16a2c-2c91-4f78-ab0e-d1db9da448a0.png)

13. Проверить, что 1-й элемент параметра salary равен salary*2 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451066-f5afd06b-fab8-4dc6-82fd-2d4bef6e493f.png)

14. Проверить, что 2-й элемент параметра salary равен salary*3 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451075-4add3ab1-96f7-4b69-9c77-0b2abf7d2c95.png)

15. Создать в окружении переменную name
16. Создать в окружении переменную age
17. Создать в окружении переменную salary

![image](https://user-images.githubusercontent.com/83454778/168451119-cc3b307d-1b9e-4975-8192-bde3bbc2903f.png)

18. Передать в окружение переменную name

      pm.environment.set("name", query.name);

19. Передать в окружение переменную age

      pm.environment.set("age", query.age);
  
20. Передать в окружение переменную salary

      pm.environment.set("salary", query.salary);

![image](https://user-images.githubusercontent.com/83454778/168451343-d5acdc33-a750-41ae-9e79-e4e24024f777.png)

21. Написать цикл который выведет в консоль по порядку элементы списка из параметра salary.

      jsonData.salary.forEach(item => console.log(item))

http://162.55.220.72:5005/user_info_2
1. Вставить параметр salary из окружения в request
2. Вставить параметр age из окружения в age
3. Вставить параметр name из окружения в name

![image](https://user-images.githubusercontent.com/83454778/168451451-111544c6-68d0-4ebd-9415-c17e7997a7b6.png)

4. Отправить запрос.
5. Статус код 200

![image](https://user-images.githubusercontent.com/83454778/168451454-73a526c1-64dd-4c49-8d18-bb2db4da22ff.png)

6. Спарсить response body в json.

      let jsonData = pm.response.json();
  
7. Спарсить request.

      let query = request.data
  
8. Проверить, что json response имеет параметр start_qa_salary

![image](https://user-images.githubusercontent.com/83454778/168451552-5bb650e7-d5fc-4a6d-b1a1-fe2f2983c9f5.png)

9. Проверить, что json response имеет параметр qa_salary_after_6_months

![image](https://user-images.githubusercontent.com/83454778/168451563-c50f3aa8-7303-4ae1-93ff-7a4745c9c5d3.png)

10. Проверить, что json response имеет параметр qa_salary_after_12_months

![image](https://user-images.githubusercontent.com/83454778/168451585-365d1003-e66d-499c-810f-514658e04ddb.png)

11. Проверить, что json response имеет параметр qa_salary_after_1.5_year

![image](https://user-images.githubusercontent.com/83454778/168451601-15a2baca-f60c-4c84-8593-39001347dca1.png)

12. Проверить, что json response имеет параметр qa_salary_after_3.5_years

![image](https://user-images.githubusercontent.com/83454778/168451618-2224843e-e225-42b5-ae6c-cd7d3cce5099.png)

13. Проверить, что json response имеет параметр person

![image](https://user-images.githubusercontent.com/83454778/168451639-5f40af2b-7484-4a29-8d10-ee35a0ccf66a.png)

14. Проверить, что параметр start_qa_salary равен salary из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451699-2e963509-839a-4b44-a35a-fe655170e0b4.png)

15. Проверить, что параметр qa_salary_after_6_months равен salary*2 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451715-d099b0b7-f8b1-4520-bf88-5a077987e9b0.png)

16. Проверить, что параметр qa_salary_after_12_months равен salary*2.7 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451737-555ab881-604f-477e-99e4-90d96f871a07.png)

17. Проверить, что параметр qa_salary_after_1.5_year равен salary*3.3 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451840-aeee1643-91fe-4518-b036-3b041404127f.png)

18. Проверить, что параметр qa_salary_after_3.5_years равен salary*3.8 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451852-d45eab2a-5024-455f-9ff7-22443ff597cc.png)

19. Проверить, что в параметре person, 1-й элемент из u_name равен salary из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451888-a2f8df91-9627-4a6f-a1e0-8ad86312a6ba.png)

20. Проверить, что что параметр u_age равен age из request (age забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451904-1339172a-7c6d-42af-8182-9d8d8b89e733.png)

21. Проверить, что параметр u_salary_5_years равен salary*4.2 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/83454778/168451930-e9329470-dac5-4c60-8fc7-1fd45a24cf25.png)

22. ***Написать цикл который выведет в консоль по порядку элементы списка из параметра person.

        for (let item in jsonData.person) {
          if(jsonData.person.hasOwnProperty(item)){
            console.log(item)
          }
        }
    
 ![image](https://user-images.githubusercontent.com/83454778/168462804-ebde45fc-89f5-426f-a5e7-55063432bc30.png)
   
