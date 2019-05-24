**Информационные технологии. Тестирование ПО. Лабораторная работа №1**

**Задание**

На основе представленных требований разработать набор тестов с примерами конкретных входных данных для обеспечения достаточного тестового покрытия, используя техники анализа граничных значений и эквивалентных классов.

**Требования**

Вариант 1. 

Поле "Пользователь":	
- применяется маска: Фамилия_Имя
- чувствительность к регистру: есть
- допустимые символы: [А-я], [A-z], [-_'`пробел]
- длина: 256 символов

Кнопка "Сохранить". Действие по нажатию: 
- при допустимом значении поля «Пользователь»: уведомление «Сохранено»
- при недопустимом значении поля «Пользователь»: уведомление «Ошибка»

**Результат**

	Соообщение "Сохранено" при следующих значениях поля "Пользователь":
	- Маск_Илон
	- Mask_Ilon
	- Ilon_Mask
	- Ma-'`_sk_Ilon
	- Ая_Az
	- Ван Гог_Винсент
	- a_a
	- n_rinICvZSffDsWAUVsjEAxmmdiMhDYpYurEpjpJARDKAWHtLmvdIpZXlCHgLkOPhLnMKGcMnkQOAFyIROqjIRNBYdezmhqCAfeiZBRWyKawXSWTCMOtquvdmAAaopiuMfmUpUeztKqURjRJmtyvqPlsMQsLEaFeBtzyfikJPfsbJKfAftgvmDbUoOSJnzQMkrjykpYFGLnadNnbUQzSdJiJNaSwzTKFYvzVldiiTRhVxtTskxeRJmgNoPBagUsG 
	(256 символов)
	Сообщение "Ошибка" при следующих значениях поля "Пользователь":
	- ilon_Mask
	- Ilon_mask
	- ilon_mask
	- I12345_N67890
	n_rinICvZSffDsWAUVsjEAxmmdiMhDYpYurEpjpJARDKAWHtLmvdIpZXlCHgLkOPhLnMKGcMnkQOAFyIROqjIRNBYdezmhqCAfeiZBRWyKawXSWTCMOtquvdmAAaopiuMfmUpUeztKqURjRJmtyvqPlsMQsLEaFeBtzyfikJPfsbJKfAftgvmDbUoOSJnzQMkrjykpYFGLnadNnbUQzSdJiJNaSwzTKFYvzVldiiTRhVxtTskxeRJmgNoPBagUsG7
	(257 символов)
	- a
	- a-a
	- Mask_Ilon2
	- |/\,;:_&<>^*?«»()
	- 
	(Пустой ввод)
	
	-      
	(Только пробелы)
	
	- _
	(Просто подчеркивание)
	
	- a_
	- _a
	- ò-âãä
	
