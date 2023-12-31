# <font size = 5 color = #00FF00> <center>PROJECT-4. Classification problem</center></font> 



##  <font color = #9ACD32> Содержание </font>

[1. Введение](https://github.com/DmitVasilev/Project-_4_-ML#-1-%D0%B2%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-)   
[2. Описание задачи](https://github.com/DmitVasilev/Project-_4_-ML#2-%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B7%D0%B0%D0%B4%D0%B0%D1%87%D0%B8)   
[3. Описание данных](https://github.com/DmitVasilev/Project-_4_-ML#3-%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)   
[4. Результат](https://github.com/DmitVasilev/Project-_4_-ML#4-%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82)                  
[5. Выводы](https://github.com/DmitVasilev/Project-_4_-ML#5-%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B)

### <font color = #9ACD32> 1. Введение </font>

Банк предоставил данные о последней маркетинговой кампании, задачей которой было привлечь клиентов для открытия депозита. Необходимо проанализировать эти данные, выявить закономерность и найти решающие факторы, повлиявшие на то, что клиент вложил деньги именно в этот банк. 
                          
:arrow_up:[к содержанию](https://github.com/DmitVasilev/Project-_4_-ML#-%D1%81%D0%BE%D0%B4%D0%B5%D1%80%D0%B6%D0%B0%D0%BD%D0%B8%D0%B5-)  

###  <font color = #9ACD32>2. Описание задачи</font>

Бизнес-задача: определить характеристики, по которым можно выявить клиентов, более склонных к открытию депозита в банке, и за счёт этого повысить результативность маркетинговой кампании.

Техническая задача для вас как для специалиста в Data Science: построить модель машинного обучения, которая на основе предложенных характеристик клиента будет предсказывать, воспользуется он предложением об открытии депозита или нет.

Проект состоит из пяти частей:
1. Первичная обработка данных 
2. Разведывательный анализ данных 
3. Отбор и преобразование признаков 
4. Решение задачи классификации: логистическая регрессия и решающие деревья
5. Решение задачи классификации: ансамбли моделей и построение прогноза

:arrow_up:[к содержанию](https://github.com/DmitVasilev/Project-_4_-ML#-%D1%81%D0%BE%D0%B4%D0%B5%D1%80%D0%B6%D0%B0%D0%BD%D0%B8%D0%B5-)  
                     
###  <font color = #9ACD32>3. Описание данных</font>

В проекте используется датасет, в котором содержатся сведения о 11162 результатах последней маркетинговой кампании среди конкретных клиентов банка. Исходная версия датасета содержит 17 полей со следующей информацией:

Данные о клиентах банка:

        age (возраст);
        job (сфера занятости);
        marital (семейное положение);
        education (уровень образования);
        default (имеется ли просроченный кредит);
        housing (имеется ли кредит на жильё);
        loan (имеется ли кредит на личные нужды);
        balance (баланс).

Данные, связанные с последним контактом в контексте текущей маркетинговой кампании:

        contact (тип контакта с клиентом);
        month (месяц, в котором был последний контакт);
        day (день, в который был последний контакт);
        duration (продолжительность контакта в секундах).

Прочие признаки:

        campaign (количество контактов с этим клиентом в течение текущей кампании);
        pdays (количество пропущенных дней с момента последней маркетинговой кампании до контакта в текущей кампании);
        previous (количество контактов до текущей кампании)
        poutcome (результат прошлой маркетинговой кампании).

И, разумеется, наша целевая переменная deposit, которая определяет, согласится ли клиент открыть депозит в банке. Именно её мы будем пытаться предсказать в данном кейсе.
                     
:arrow_up:[к содержанию](https://github.com/DmitVasilev/Project-_4_-ML#-%D1%81%D0%BE%D0%B4%D0%B5%D1%80%D0%B6%D0%B0%D0%BD%D0%B8%D0%B5-)   



###  <font color = #9ACD32>4. Результат</font>

Ноутбук с решением на GitHub: [Project_4_ML.ipynb](https://github.com/DmitVasilev/Project-_4_-ML/blob/95c158fb6df7cca03a6ea1a843e72b43a4631f79/Project_4_ML.ipynb).     
 
Обеспечить воспроизводимость кода поможет файл requirements.txt: [requirements.txt](https://github.com/DmitVasilev/Project-_4_-ML/blob/95c158fb6df7cca03a6ea1a843e72b43a4631f79/requirements.txt). 
                        
:arrow_up:[к содержанию](https://github.com/DmitVasilev/Project-_4_-ML#-%D1%81%D0%BE%D0%B4%D0%B5%D1%80%D0%B6%D0%B0%D0%BD%D0%B8%D0%B5-)      


###  <font color = #9ACD32>5. Выводы</font>

В данном проекте была проведена работа по решению задачи классификации клиентов банка по признаку согласия/не согласия на открытие депозита. 
В проекте использованы модели логистической регрессии, дерева решений, случайного леса, градиентного бустинга и стекинга. Проведен подбор оптимальных значений гиперпараметров с использованием GridSearchCV и Optuna. Достигнутое значение метрики f1-score 0.82 для модели случайного леса.
                             
:arrow_up:[к содержанию](https://github.com/DmitVasilev/Project-_4_-ML#-%D1%81%D0%BE%D0%B4%D0%B5%D1%80%D0%B6%D0%B0%D0%BD%D0%B8%D0%B5-)   