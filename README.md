Лабораторная работа 8. Повышение удобства использования приложений
Цель работы
Изучение средств для повышения удобства работы пользователей и
получение навыков по созданию контекстной справки, всплывающей
подсказки, а также файлов со справочной информацией.
Упражнение 1. Создание контекстной справки
1.	Откройте Windows-приложение WinAsynchMethod.
Открыл
2.	Откройте форму в режиме конструктора.
![image](https://github.com/user-attachments/assets/5d4f4565-3b31-4654-8ec2-446579f7cef7)
3.	Выберите пункт меню ViewToolBox.
   ![image](https://github.com/user-attachments/assets/945437b4-0d7c-4a51-8c16-74062b921d2c)
4. Добавьте ЭУ HelpProvider на форму.
   ![image](https://github.com/user-attachments/assets/432b3f93-0550-4d25-934a-f74e8582320d)
5. Выделите поле txbA для отображения ее свойств.
Выделил
![image](https://github.com/user-attachments/assets/c1e57b6f-d45d-4224-8d7a-cf38ddd51e1a)
6. Для свойства HelpString on helpProvider1 задайте значение For
input integer A.
![image](https://github.com/user-attachments/assets/a6eeb788-c805-4793-8d75-043abbfdf7b6)
7. Постройте и запустите приложение.
Снова не получилось
![image](https://github.com/user-attachments/assets/17a3d0ec-f266-4c57-8477-86958df8b023)
8. Переместитесь по форме, используя клавишу Tab, до тех пор, пока
поле txbA не окажется в фокусе.
Переместился
![image](https://github.com/user-attachments/assets/0605473d-b371-42e3-8fe4-9e5cd439550a)
9. Нажмите на клавишу F1 для отображения контекстной справки
для поля txbA.
![image](https://github.com/user-attachments/assets/1d1588ac-7deb-4607-996b-a60f03aff1d6)
Создайте подобную функциональность на форме проекта
WinAsynchMethod:
1.	Добавьте к имеющимся свойствам формы следующие свойства:
![image](https://github.com/user-attachments/assets/822fccc7-50fc-488c-ba02-946aa0f2cc53)
![image](https://github.com/user-attachments/assets/b54709c6-4ec3-4964-a8f2-7a56796e9556)
![image](https://github.com/user-attachments/assets/b59992b8-d1bb-46c3-afa6-0abd09bdce55)
Добавил
2. Для полей ввода txbA, txbB и двух кнопок в свойстве ShowHelp on
helpProvider1 каждого из этих элементов установите значение True.
txbA -   ![image](https://github.com/user-attachments/assets/ca10c52d-e615-48d8-8a6b-7c5ce681b6f3)
txbB -  ![image](https://github.com/user-attachments/assets/6000c93b-baee-4e22-ae15-1b9da8b3c9b6)
3. Текст, введенный в поле свойства HelpString on helpProvider1,
будет появляться в качестве подсказки для конкретного элемента.
Установите следующие значения этого свойства для каждого элемента:
![image](https://github.com/user-attachments/assets/96ec5dfa-13f6-41ca-82e6-7ceb16ddc6e5)
![image](https://github.com/user-attachments/assets/60c33d3f-49af-40e9-b05b-288292a4d9bd)
![image](https://github.com/user-attachments/assets/641c62ca-55ac-4275-adc1-bbd81a0e5df7)
![image](https://github.com/user-attachments/assets/cd4b1fe8-3377-495e-b4f1-8e4c991d8c92)
![image](https://github.com/user-attachments/assets/052ef4c9-b787-4c3e-92f3-28d221eeca4c)
4.	Постройте и запустите приложение.
   Не получилось
  	![image](https://github.com/user-attachments/assets/7022bc45-29f5-4990-8a37-cb1150041680)
5. Для активации контекстной справки нажмите на кнопку “?”,
расположенную в правом верхнем углу приложения.
![image](https://github.com/user-attachments/assets/1f20b5a6-c72a-4c7b-b43e-dc13d7ccd9e0)
Нажал
6. Нажмите на любую кнопку, появится маленькое окошко,
объясняющее, что происходит при ее нажатии.
Нажал, и под каждом элементом появилась маленькая контекстная справка, при наведении курсора на какой-либо элемент.
Упражнение 2. Использование справочного файла
1.	Откройте Windows-приложение WinAsynchMethod.
Открыл
2. Откройте форму в режиме конструктора.
   ![image](https://github.com/user-attachments/assets/2c993f27-8f44-4875-b6a8-a640925f2e3d)
3. Выберите пункт меню ViewToolBox.
   ![image](https://github.com/user-attachments/assets/6bbb1aa4-6403-4cfe-90b9-b7f96daaf0d1)
4. Добавьте ЭУ HelpProvider на форму (если он не был добавлен
ранее).
HelpProvider добавлен
![image](https://github.com/user-attachments/assets/f31f8e4b-7f8e-4837-9a09-82d1806c6b97)
5. В папке с решением создайте файл справки, например, документ
Microsoft Word. Текст укажите произвольный.
![image](https://github.com/user-attachments/assets/21430700-f775-4cc0-9a8d-93a359846333)
6. Для элемента helpProvider1 в свойстве HelpNamespace укажите
путь к файлу справки.
Не получилось, тк он не видит файл
![image](https://github.com/user-attachments/assets/11c6bce1-29ab-479d-b5f0-7d937ab5f63d)
7. Реализуйте возможность вызова файла справки созданием либо
команды меню, либо кнопки (и команда меню и кнопка может называться,
например, help).
Не получилось
8. Создайте обработчик события выбора файла справки. В теле
обработчика укажите следующую строку:
Help.ShowHelp(this,helpProvider1.HelpNamespace);
![image](https://github.com/user-attachments/assets/23eb44f3-ab41-48ac-9564-bbbc1463eb83)
пусть будет так
9. Постройте и запустите приложение.
    ![image](https://github.com/user-attachments/assets/4cf5b372-f13d-4892-84fd-397f24930698)
10. Выберите команду вызова справки. Проверьте, что открылся
требуемый файл.
Нет, не открылся

Упражнение 3. Добавление всплывающих подсказок
1. Откройте Windows-приложение WinAsynchMethod в режиме
конструктора.
Открыл

2.	Выберите пункт меню ViewToolBox.
Выбрал

3.	Добавьте на форму элемент управления ToolTip.
Добавил
![image](https://github.com/user-attachments/assets/c0adf919-4f49-4a90-bff3-4410b4d39a3b)
4. В окне Properties расположенных на форме элементов и в самой
форме появилось свойство ToolTip on toolTip1. Установите следующие
значения этого свойства для каждого из элементов:
![image](https://github.com/user-attachments/assets/d9e72d56-4dfa-4fe7-91eb-3eaa622c6463)
txbA -  ![image](https://github.com/user-attachments/assets/abe53799-6932-49d8-9cf4-798d8f1a2334)
txbB -  ![image](https://github.com/user-attachments/assets/83e8bec7-c445-4f60-b35f-e97685e44fd0)
btnRun -  ![image](https://github.com/user-attachments/assets/c61dbf3c-ff80-4d5a-8f63-86865a3ecff6)
btnWork - ![image](https://github.com/user-attachments/assets/71ee67e8-2374-4de0-9902-4ff056d1127b)
5. Постройте и запустите приложение. Проверьте, что при наведении
курсора на элемент управления появляется его подсказка.
![image](https://github.com/user-attachments/assets/d4f4b567-b09a-4066-9131-d02f5bb2bad9)
![image](https://github.com/user-attachments/assets/e5308081-4265-485b-81c4-ac830b24a69d)
- запустил, но на этот раз, никаких подсказок не появляется…
Упражнение 4. Автоматический выбор языка при запуске приложения
1. Создайте новое Windows-приложение и назовите его WinLanguage.
![image](https://github.com/user-attachments/assets/5ca3f3ea-82fd-4626-aa8d-b52983507dbc)
2.	Добавьте на форму кнопку и главное меню.
   ![image](https://github.com/user-attachments/assets/9eaf0de7-8c8b-41a9-ad3c-d4edc0ea6645)
3. Установите следующие значения свойства Text для элементов:
главное меню – menu,
первая команда – command one,
вторая команда – command two,
кнопка – Close,
для самой формы – Form.
![image](https://github.com/user-attachments/assets/cda6954f-6450-498a-91c3-b9a131a56504)
4. Для кнопки реализуйте обработчик, закрывающий форму:
this.Close();
![image](https://github.com/user-attachments/assets/b5450d38-7b03-4de7-bdc3-b2ea2c1885dd)
5. Для формы установите свойству Localizable значение True. Это
свойство разрешает поддержку многоязычного интерфейса.
![image](https://github.com/user-attachments/assets/a148f026-04f8-4be1-a64a-11b3ed2b1197)
6. В свойстве Language выберите значение English (United States).
   ![image](https://github.com/user-attachments/assets/28ccfdc4-70f7-41c1-ab1f-d3d3ea3b4146)
7. Постройте приложение. В итоге получилась версия программы с
интерфейсом на английском языке.
![image](https://github.com/user-attachments/assets/ad775a73-9802-4dc2-baec-9ec6e35407a2)
8. В свойстве Language выберите Russian (Russia).
   ![image](https://github.com/user-attachments/assets/c338d079-b563-4a45-96cd-70a0a6af6d02)
9. Измените свойство Text элементов, заменив названия на
английском языке соответствующими названиями на русском.
![image](https://github.com/user-attachments/assets/dc07fc8a-8ef9-4110-bdb7-b4dc1832025c)
Ничего не изменилось, как было на русском, так и осталось…
10. Перейдите в код формы и подключите пространство имен
Threading:
using System.Threading;
![image](https://github.com/user-attachments/assets/cad9306a-e949-4ec6-9e20-b5755ca7282a)
11. В конструкторе формы до InitializeComponent(); установите
культуру пользовательского интерфейса равной текущей культуре:
Thread.CurrentThread.CurrentUICulture =
Thread.CurrentThread.CurrentCulture
![image](https://github.com/user-attachments/assets/c666e90a-30e4-42e7-862f-6b5b88d96ac2)
12. Постройте и запустите приложение. Среда CLR проверяет
установленный язык и выводит приложение с интерфейсом на языке,
установленном на вкладке "Региональные параметры" в настройках
инструмента "Язык и региональные параметры".
![image](https://github.com/user-attachments/assets/8418a92d-b76c-4146-8b1f-c05118a4d31c)
Сколько бы я не изменял язык, ничего не происходит.
13. Закройте приложение. Перейдите в "Панель управления" и
установите другой язык (например, "Английский (США)") на вкладке
"Региональные параметры" в настройках инструмента "Язык и
региональные параметры". Снова запустите приложение. Теперь
интерфейс приложения должен быть на другом языке (например,
английском).
Снова ничего не получилось
14. При локализации приложения среда Visual Studio .NET создает
сборку, в которой хранятся все данные о приложении. В окне Solution
Explorer нажмите на кнопку (Show All Files) для просмотра добавленных
файлов. Названия файлов-ресурсов (Form1. en-US и Form1.ru-RU)
содержат в себе указание на язык (первая часть – en или ru) и регион
(вторая часть US или RU).
….
Упражнение 5. Локализация приложения
Локализация формы Windows-приложения
1. Откройте стартовый проект UsabilityDemo.sln из папки
install_folder\Practices\Mod08\Mod08_04\Starter_2008
Я не понимаю, о каком проекте идет речь…
Поэтому, я открыл проект WinAsynchMethod
2. Откройте файл UsabilityDemo.cs в режиме конструктора.
В моем случае Form1.cs
![image](https://github.com/user-attachments/assets/6ed78f65-e177-4a69-ba27-bbd91427d78f)
3. Нажмите на кнопку Show All Files в окне Solution Explorer.
Нажал
4. Обратите внимание на значение свойства формы Localizable. Оно
установлено в True, что означает, что форма может быть локализована.
![image](https://github.com/user-attachments/assets/32793596-a7e9-49a4-8796-928ce9700703)
5. Для свойства формы Language задайте значение French(France).
   ![image](https://github.com/user-attachments/assets/7225f9fb-1c5e-44cf-8512-cb4f25553b64)
6. Для свойства формы Text задайте значение Démonstration de
l'utilisation.
![image](https://github.com/user-attachments/assets/5cdd2bd6-4ca4-4750-9aa7-f1c95c7010a0)
7. Для свойства Text меню Help и пункта меню Help задайте
значение Aide.
Не понял..
8. Для свойства Text кнопки Choose a Culture задайте значение
Choisir une langue
![image](https://github.com/user-attachments/assets/cbdefd4e-fc8b-4117-ba37-42026f63098a)
пришлось изменить названия кнопок на проекте, тк добавить новые, на этот же проект – не получилось
9. Для свойства Text кнопки Show Date/Time задайте значение
Afficher la date/l'heure.
В моем случае, кнопка Choose
![image](https://github.com/user-attachments/assets/39d7409d-4a7d-4347-b9e9-b252d7f2116a)
![image](https://github.com/user-attachments/assets/47357cb9-20c6-40c9-adfb-339466c38fec)
10. Для свойства Text кнопки Show Currency задайте значение
Afficher la devise.
В моем случае, кнопка Culture
![image](https://github.com/user-attachments/assets/f4528ca8-6d40-4163-a46c-cf4cd711d05d)
11. Для свойства Text кнопки Show a String задайте значение Afficher
une chaîne.
А это я уже от себя добавил
![image](https://github.com/user-attachments/assets/229b0226-8fa4-474c-a7ce-a6338b0a5405)
12. Для свойства Text кнопки Exit задайте значение Quitter.
И это тоже
![image](https://github.com/user-attachments/assets/77329e5e-4051-4484-963c-28b27608248a)
Добавление в приложение файл строковых ресурсов
1. В окне Solution Explorer ПКМ по проекту UsabilityDemo | Add |
Add New Item.
В моем случае к моему проекту
Выбираю….
2. В окне Add New Item выберите Assembly Resource File.
   ![image](https://github.com/user-attachments/assets/f3a6b2ba-3120-4d30-a12c-4bc2c5fe2545)
3. Задайте для файла ресурсов имя UsabilityDemoText.fr-FR.resx и
нажмите на кнопку Open.
![image](https://github.com/user-attachments/assets/ae690c1d-bc37-480b-b4b6-a5974906bf5a)
4. В строке ресурсов задайте для Name значение SimpleTextString.
   ![image](https://github.com/user-attachments/assets/074c5fe4-ceda-435e-a4c9-f1d3c50a500f)
А вот тут я уже запутался…
5. В строке ресурсов задайте для Value значение Voici du texte.
Ничего не получилось, тк я использовал прошлый проект.
6. Сохраните и закройте файл ресурсов.
Добавление кода для получения значений строковых
1. Откройте файл с кодом UsabilityDemo.cs.
В моем случае Form1.cs
![image](https://github.com/user-attachments/assets/d6f8256d-6bc9-4fba-93b8-4c655a912866)
2. В окне Task List отобразите комментарии TODO. Для этого
выберите пункт меню View | Show Tasks | All.
![image](https://github.com/user-attachments/assets/44db8dff-960d-4e6d-bcab-521c8a428877)
Ничего не показывает
3. Добавьте три директивы using, для возможности поддержки
локализации приложения.
using System.Globalization;
using System.Resources;
using System.Threading;
![image](https://github.com/user-attachments/assets/a4c63725-77a9-44c4-a80a-44c197ebe63d)
4. Найдите в коде второй комментарий TODO. Объявите private
переменную типа ResourceManager.
private ResourceManager RM;
Поставил в рандомное место
![image](https://github.com/user-attachments/assets/b4f664b7-8233-4f02-a567-2c29d745cb6c)
5. Найдите в коде следующий комментарий TODO. Создайте
экземпляр класса ResourceManager. Код добавляется в первый
конструктор приложения:
RM = new ResourceManager("UsabilityDemo.UsabilityDemoText",
Assembly.GetExecutingAssembly());
Его я тоже не нашел, поэтому, поставил наугад
![image](https://github.com/user-attachments/assets/e8fef6fc-9f43-4330-b3fa-e6a0148517da)
6. Найдите в коде следующий комментарий TODO. Создайте
экземпляр класса ResourceManager. Код добавляется во второй
конструктор приложения:
RM = new ResourceManager("UsabilityDemo.UsabilityDemoText",
Assembly.GetExecutingAssembly());
![image](https://github.com/user-attachments/assets/4ca1ef61-87c1-4292-9f8a-3e1d68114519)
7. Найдите в коде следующий комментарий TODO. Добавьте код
использования менеджера ресурсов для получения строки текста из файла
ресурсов и отображения ее в текстовом поле.
OutputTextBox.Text = RM.GetString("SimpleTextString");
Снова поставил в рандомное место
![image](https://github.com/user-attachments/assets/aa68562c-41e7-441e-b76c-2754167f70cb)
Поставил запятую, чтобы не обозначалось ошибкой
8. Найдите в коде следующий комментарий TODO. Добавьте код для
задания свойствам Culture и UICulture значений, выбранных
пользователем.
Thread.CurrentThread.CurrentUICulture = new
CultureInfo(ChosenCulture, false);
Thread.CurrentThread.CurrentCulture = new
CultureInfo(ChosenCulture, false);
![image](https://github.com/user-attachments/assets/799f9391-47b2-4f24-94a7-23752d64209e)
Снова запутался
9. Сохраните проект.

Тестирование работы приложения
1.	Постройте и запустите приложение.
![image](https://github.com/user-attachments/assets/7ede287a-ab0e-43de-831e-9f99c9d7edcf)
Запустил
