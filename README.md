# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #1 выполнил:
- Султанов Егор Альбертович
- РИ-210948
Отметка о выполнении заданий:

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | # | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

## Цель работы
Ознакомиться с основными операторами зыка Python на примере реализации линейной регрессии.

## Задание 1

### -Сохранить документ google.colab на свой диск с запуском программы, выводящей сообщение "Hello World". Привести скриншоты


![0VoEdD7CXTY](https://user-images.githubusercontent.com/91984484/191815303-feee3d5a-3f3b-4582-81e3-f3fb176950ac.jpg)


![eBVLzJWXyyw](https://user-images.githubusercontent.com/91984484/191895780-df39a31c-4905-409e-8dd1-47e6f4e7e321.jpg)

### -Привести скриншоты вывода сообщение "Hello World" в консоли Unity.


## Задание 2
### Пошагово выполнить каждый пункт раздела "ход работы" с описанием и примерами реализации задач:
#### 1. Произвести подготовку данных для работы с алгоритмом линейной регрессии. 10 видов данных были установлены случайным образом, и данные находились в линейной зависимости. Данные преобразуются в формат массива, чтобы их можно было вычислить напрямую при использовании умножения и сложения.



![1](https://user-images.githubusercontent.com/91984484/191910835-19cf9217-45cf-4417-b88a-cd77b29cf3b0.jpg)



#### 2. Определите связанные функции. Функция модели: определет модель линейной регрессии wx+b. Функция потерь: функция потерь среднеквадратичной ошибки. Функция оптимизации: метод градиентного спуска для нахождения частных производных w и b.



![2](https://user-images.githubusercontent.com/91984484/191913676-d18b3f76-18f0-4022-a550-92822c750bed.jpg)



#### 3. Начать итерацию
- Шаг 1 Инициализация и модель итеративной оптимизации



![3](https://user-images.githubusercontent.com/91984484/191914612-adfc0a1a-6e48-4d81-a8f2-0353b5ecac02.jpg)



- Шаг 2 На второй итерации отображаются значения параметров, значения потерь и эффекты визуализации после итерации



![C_5DcEPkQPU](https://user-images.githubusercontent.com/91984484/191915016-1deafb63-a79b-46ba-b1dd-9fbfece8cb69.jpg)



- Шаг 3 Третья итерация показывает значения параметров, значения потерь и эффекты визуализации после итерации



![0I4VtDCECAs](https://user-images.githubusercontent.com/91984484/191915249-561139ce-1fcc-47d1-b1d5-8c838c50910f.jpg)



- Шаг 4 На четвертой итерации отображаются значения параметров, значения потерь и эффекты визуализации после итерации



![8IV7IrOgePU](https://user-images.githubusercontent.com/91984484/191915405-213189b4-8063-4e4c-b43b-3e6c45fa7f95.jpg)



- Шаг 5 Пятая итерация показывает значения параметров, значения потерь и эффекты визуализации после итерации



![tVnb1ky28Sc](https://user-images.githubusercontent.com/91984484/191915553-c2c39d98-608d-4bd1-bf13-6a48c7c5fd0b.jpg)



- Шаг 6 10000-я итерация, показывающая значения параметров, потери и визуализацию после итерации



![9XsFFSWPFiI](https://user-images.githubusercontent.com/91984484/191915823-251ad8ea-13c2-4453-b523-c4b3ef1edc9e.jpg)




## Задание 3
### Должна ли величина loss стремиться к нулю при изменении исходных данных? Ответьте на вопрос, приведите пример выполнения кода, который подтверждает ваш ответ.


- Перечисленные в этом туториале действия могут быть выполнены запуском на исполнение скрипт-файла, доступного [в репозитории](https://github.com/Den1sovDm1triy/hfss-scripting/blob/main/ScreatingSphereInAEDT.py).
- Для запуска скрипт-файла откройте Ansys Electronics Desktop. Перейдите во вкладку [Automation] - [Run Script] - [Выберите файл с именем ScreatingSphereInAEDT.py из репозитория].

```py

import ScriptEnv
ScriptEnv.Initialize("Ansoft.ElectronicsDesktop")
oDesktop.RestoreWindow()
oProject = oDesktop.NewProject()
oProject.Rename("C:/Users/denisov.dv/Documents/Ansoft/SphereDIffraction.aedt", True)
oProject.InsertDesign("HFSS", "HFSSDesign1", "HFSS Terminal Network", "")
oDesign = oProject.SetActiveDesign("HFSSDesign1")
oEditor = oDesign.SetActiveEditor("3D Modeler")
oEditor.CreateSphere(
	[
		"NAME:SphereParameters",
		"XCenter:="		, "0mm",
		"YCenter:="		, "0mm",
		"ZCenter:="		, "0mm",
		"Radius:="		, "1.0770329614269mm"
	], 
)

```
### Какова роль параметра Lr? Ответьте на вопрос, приведите пример выполнения кода, который подтверждает ваш ответ. В качестве эксперимента можете изменить значение параметра.

#### Параметр Lr играет роль коэфициента отклонения. Если он будет слишком большим, программа работать не будет, и вот тому пример:

![GoBqAdbDIX4](https://user-images.githubusercontent.com/91984484/191919311-d4d5f4df-b6a2-4152-b023-ee4888d06d70.jpg)


#### А если параметр Lr будет слишком маленьким, то данные будут некорректные:

![GL-pQMui38Q](https://user-images.githubusercontent.com/91984484/191921581-3b035116-59f6-4626-8e0e-5dcdd15d3653.jpg)


## Выводы
### В результате работы:
- освежил знания работы в Python
- поработал в среде разработки Unity
- написал простейший код на языке C# и Python
- проанализировал величину loss 
- узнал роль параметра Lr

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
