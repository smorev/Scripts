﻿# Содержание

## [Общие сведения](#common_info)  
### [Демонстрационные примеры БАЗИС-скрипт](#demo_samples)  
### [Редактор скриптов](#script_editor)  
#### [Запуск редактора](#launch_editor)  
#### [Интерфейс Редактора скриптов](#script_editor_interface)
#### [Команды редактора](#script_editor_menu)
#### [Вкладка скрипта](#script_editor_tab)

## [Организация взаимодействия с пользователем](#user_interface)
### [Элементы управления на панелях инструментов](#dynamic_controls)
### [Элементы управления вспомогательной панели Свойства](#property_controls)
### [Выдача сообщений пользователю](#user_messages)

## [Синтаксис языка](#language_syntax)
### [Список ключевых слов языка программирования БАЗИС-Script](#keywords)
### [Список зарезервированных слов](#reserved_words)
### [Комментарии](#comments)
### [Переменные](#variables)
### [Константы](#constants)
### [Арифметические операции](#arithmetic_ops)
### [Логические операции](#logical_ops)
### [Операции сравнения](#compare_ops)
### [Оператор if...else](##if_else)
### [Оператор switch](#switch)
### [Оператор условного выражения](#conditional_op)
### [Операторы break и continue](#break_continue)
### [Цикл for](#for_cycle)
### [Цикл while](#while_cycle)
### [Цикл do...while](#do_while_cycle)
### [Оператор with](#with_op)
### [Оператор try...catch...throw](#exception_handling)
### [Функции](#functions)

## [Общее для всех модулей](#common_variables)
### [Глобальные константы](#global_consts)
<!--
AxisX
AxisY
AxisZ
Axis_X
Axis_Y
Axis_Z
-->
### [Глобальные перечисляемые типы](#global_enums)
<!--
TProjection3dEnum
PanelSideEnum 
SalonAnimationType
TextureDir
WindowPosition
FurnSchemeType
SchemeFurnPos
ErrorType
DatumMode
FurniturePosition
ElementType
FurnPositionMode
-->
[//]: # (Глобальные свойства и методы)
### [Глобальные свойства](#global_props)
<!--
system
Model
Action
ActiveMaterial
AnimationType
-->
### [Глобальные методы](#global_methods)
<!--
prompt
alert
confirm
OpenFurniture
SelectAll
UnSelectAll
ViewAll
SetCamera
GetPoint
GetObject
GetPanel
GetEdge
AddPanel
AddFrontPanel
AddHorizPanel
AddVertPanel
AddExtrusion
AddTrajectory
AddBlock
AddAssembly
AddDraftBlock
AddCopy
DeleteNewObjects
DeleteObject
StartEditing
BeginBlock
EndBlock
NewButtonInput
NewFloatInput
NewNumberInput
NewMaterialInput
NewButtMaterialInput
NewFurnitureInput
FormatMatName
OrientCamera
ExtractMatName
ExtractMatCode
NewVector
NewPoint
NewContour
NewCOMObject
NewForm
-->
## [Общие типы для всех модулей](#common_types)
### [Geometry2D](#geometry2d_class)
<!--
Методы
Intersect
Compare
Distance
Area
-->
### [System](#system_class)
<!--
Методы
include
log
fileExists
writeTextFile
askWriteTextFile
readTextFile
askReadTextFile
secureExec
exec
getFileName
getFileNameWithoutExtension
askFileNameSave
askFolder
Свойства
apiVersion
developerApiVersion
-->
### [Model3D](model3d_class)
<!--
Свойства
Selected
SelectionCount
Selections
Count
Objects
-->
### [Action3D](action3d_class)
<!--
Свойства
Interactive
MouseX
MouseY
Pos3
ViewDir
UpDir
RightDir
ShowPoints
ShowEdges
Hint
ErrorHint
BlinkHint
OnClick
OnMove
OnStart
OnFinish
Properties
OnRayTraceFinished
ModelFilename
Методы
Continue
Commit
Finish
Cancel
AsyncExec
BeginOrtho3
EndOrtho3
CursorToClosestPoint
CursorToClosestLine
CursorToMiddleOfLine
Find3DPoint
Find3DPointXZPlane
Get3Dobject
RayTraceScene
LoadModel
SaveModel
NewModel
NewFurniture
NewFragment
Revert
ArrangePositions
ReplaceFurniture
ChooseMaterial
-->
### [ScriptProperty](#script_prop_class)
<!--
Свойства
Name
Enabled
ChildrenEnabled
Visible
OnChange
Count
Items
Expanded
OnDeactivate
OnValueValidate
ValueValid
NameEditable
BackColor
PopupMenu
DropDownMenu
OnActivate
OnValueChange
Tag
Методы
Clear
NewCOMObject
Save
Load
NewGroup
NewImage
NewString
NewBool
NewNumber
NewButton
NewMaterial
NewButt
NewFurniture
NewColor
NewSeparator
Validate
-->
### [ScriptGroupProperty](#script_group_class)
<!--
Свойства
Image
MaxHeight
Scrollable
-->
### [ScriptStringProperty](#script_string_class)
<!--
Свойства
Value
-->
### [ScriptBooleanProperty](#script_bool_class)
<!--
Свойства
Value
-->
### [ScriptNumberProperty](#script_number_class)
<!--
Свойства
MaxValue
MinValue
ValueStep
Value
-->
### [ScriptButtonProperty](#script_button_class)
<!--
Свойства
Value
OnClick
-->
### [ScriptMaterialProperty](#script_material_class)
<!--
Свойства
Width
Методы
SetActive
-->
### [ScriptButtProperty](#script_butt_class)
<!--
Свойства
Thickness
Width
Методы
SetActive
-->
### [ScriptFurnitureProperty](#script_furn_class)
<!--
Свойства
Value
-->
### [ScriptColorProperty](#script_color_class)
<!--
Свойства
Value
-->
### [ScriptMenu](#script_menu_class)
<!--
Свойства
Name
OnChange
Count
Items
Store
Методы
Clear
Save
Load
NewGroup
NewString
NewBool
NewNumber
NewButton
-->

### [FurnMaterial](#furn_mat_class)
<!--
Свойства
Name
Thickness
Width
Методы
Make
-->
### [Vector](#vector_class)
<!--
Свойства
x
y
z
-->
### [Point](#point_class)
<!--
Свойства
x
y
-->
### [Edge3](#edge3_class)
<!--
Свойства
First
Last
GFirst
GLast
-->
### [Object3](#object3_class)
<!--
Свойства
Name
ArtPos
Owner
Visible
Selected
List
AsList
AsPanel
Position
PositionX
PositionY
PositionZ
GMax
GMin
GSize
GabMin
GabMax
UserPropCount
UserProperty
UserPropertyName
Методы
SetDefaultTransform
Translate
Rotate
TranslateGCS
RotateGCS
RotateX
RotateY
RotateZ
Orient
OrientGCS
Reflect
ToObject
ToGlobal
NToObject
NToGlobal
Build
IsOwner
-->
### [List3D](#list3d_class)
<!--
Свойства
Count
IsElastic
Objects
Методы
ElasticResize
Load
-->
### [Panel](#panel_class)
<!--
Свойства
Contour
Butts
Cuts
Plastics
ContourHeight
ContourWidth
Thickness
MaterialName
MaterialWidth
Методы
AddButt
AddCut
AddPlastic
IsButtVisible
-->
### [Extrusion](#extrusion_class)
<!--
Свойства
Contour
Thickness
MaterialName
-->
### [Trajectory](#trajectory_class)
<!--
Свойства
Contour2D
Trajectory2D
MaterialName
Пример
-->
### [Block](#block_class)
<!--
Свойства
IsFastener
-->
### [Assembly](#assembly_class)
<!--
Свойства
AnimType
-->
### [PanelButts](#panel_butts_class)
<!--
Свойства
Count
Методы
Butts[]
Add
-->
### [PanelButt](#panel_butt_class)
<!--
Свойства
ElemIndex
Sign
Material
Thickness
Width
ClipPanel
Overhung
Allowance
CutIndex
Profile
-->
### [PanelPlastics](#panel_plastics_class)
<!--
Свойства
Count
Методы
Plastics[]
Add
-->
### [PanelPlastic](#panel_plastic_class)
<!--
Свойства
Material
Thickness
TextureOrientation
-->
### [PanelCuts](#panel_cuts_class)
<!--
Свойства
Count
Методы
Add
Cuts
-->
### [PanelCut](#panel_cut_class)
<!--
Свойства
Name
Sign
Trajectory
Contour
-->
### [Contour2D](#contour2d_class)
<!--Свойства
Count
Objects
Width
Height
Min
Max
Методы
Clear
Move
Rotate
AddRectangle
AddRoundRect
AddLine
AddCircle
AddArc
AddArc3
AddEquidistantRecursive
Subtraction
Addition
RoundingEx
FacetEx
Rounding
Facet
Find
Fit
Elastic
Symmetry
Load
OrderContours
AddEquidistant
IsPointInside
IsInContour
IsClosedContour
IsContourRectangl
-->
### [InControl](#incontrol_class)
<!--
Свойства
id
Enabled
Visible
Hint
OnChange
-->
### [InButton](#inbutton_class)
<!--
Свойства
Caption
Combo
Методы
NewSubMenu
-->
### [InFloat](#infloat_class)
<!--
Свойства
Value
ReadOnly
Fixed
-->
### [InNumber](#innumber_class)
<!--
Свойства
Value
ReadOnly
Fixed
-->
### [InMaterial](#inmaterial_class)
<!--
Свойства
Name
Thickness
Width
Методы
SetActive
Apply
-->
### [InButtMaterial](#inbuttmaterial_class)
<!--
Свойства
Name
Sign
Thickness
Width
Overhung
Allowance
ClipPanel
-->
### [InFurniture](#infurniture_class)
<!--
Свойства
DatumModeFilter
DatumMode
Методы
Mount
Mount1
MountScheme
MountBox
-->
### [ModelInspector](#model_inspector_class)
<!--
Свойства
ErrorList
Options
Методы
Run
-->
### [InspectorOptions](#inspector_options_class)
<!--
Свойства
ObjIntersectionAnalyze
FastIntersectionAnalyze
FastIncorrectAnalyze
PanelNotFixedAnalyze
PanelTooLargeAnalyze
PlasticTooLargeAnalyze
MatNotExistsAnalyze
MatOutOfStockAnalyze
-->
### [InspectorError](#inspector_error_class)
<!--
Свойства
ErrorType
ErrorObjectsCount
ErrorObjects
ErrorMessage
ObjectsNames
-->
### [ImportExportSVG](#import_export_svg_class)
<!--
Свойства
CurveQuality
GroupElems
Методы
Save
Load
-->
### [ImportExport](#import_export_class)
<!--
Свойства
SVG
-->
### [InfFurniture](#furniture_info_class)
<!--
Свойства
DatumModeFilter
DatumMode
Методы
Mount
Mount1
MountScheme
MountBox
Make
EncodeToString
DecodeFromString
Choose
-->
### [RootProperties](#root_props_class)
<!--
Методы
NewFurnitureValue
-->
### [Elem2D](#elem2d_class)
<!--
Свойства
ElType
Методы
IsLine
AsLine
IsCircle
AsCircle
IsEllipse
AsEllipse
IsArc
AsArc
IsList
AsList
ObjLength
-->
### [Line2D](#line2d_class)
<!--
Свойства
Pos1
Pos2
-->
### [Arc2D](#arc2d_class)
<!--
Свойства
Pos1
Pos2
Center
ArcDir
-->
### [Circle2D](#circle2d_class)
<!--
Свойства
Center
CirRadius
Dir
-->
### [Ellipse2D](#ellipse2d_class)
<!--
Свойства
Center
MajorRadius
MinorRadius
MajorAxisAngle
Dir
-->
### [FurnArticle](#furn_article_class)
<!--
Свойства
Name
OrderCode
OrderName
DatumMode
Методы
NameWithCode
-->
## [БАЗИС-Мебельщик](#woodworker_ww)
## [Глобальные константы БАЗИС-Мебельщик](#ww_constants)
<!--
p3dFront
p3dLeft
p3dRight
p3dTop
p3dBottom
p3dIsometric
-->

## [Типы в БАЗИС-Мебельщик](#ww_types)
### [ScriptForm](#script_form_class)
<!--Свойства
Properties
Caption
Width
Height
MinWidth
MinHeight
Visible
Left
Top
OKButton
OKButtonCaption
CancelButton
CancelButtonCaption
OnClose
OnShow
Resizable
Dockable
OnOkButtonClick
OnCancelButtonClick
Методы
Show
ShowModal
Close
-->

<!--Мастер построения дверей-->
### [DoorsMaker](#doors_maker_class)
<!--
Методы
Silent
ShowErrors
Save
Load
Setup
-->
<!--Мастер построения ящиков-->
### [BoxesMaker](#boxes_maker_class)
<!--
Методы
ShowErrors
Save
Load
Setup
-->
## [БАЗИС-Смета](#estimate)
## [Глобальные свойства БАЗИС-Смета](#estimate_props)
<!--
Panel
Holes
Material
Result
Objects
-->
## [Типы в БАЗИС-Смета](#estimate_types)
### [EstimateObject](#estimate_object_class)
<!--
Методы
AsPanel
IsPanel
AsButt
IsButt
AsPlastic
IsPlastic
AsExtrusionBody
IsExtrusionBody
AsTrajectoryBody
IsTrajectoryBody
-->
### [EstimateObjectList](#estimate_objlist_class)
<!--
Свойства
Count
Items
-->
### [PanelHoles](#panel_holes_class)
<!--
Свойства
Count
Holes
-->
### [PanelHole](#panel_hole_class)
<!--
Свойства
Depth
Diameter
-->
## [БАЗИС-Салон](#salon)
## [Типы в БАЗИС-Салон](#salon_types)
### [ScItemTovarList](#tovar_items_class)
<!--
Свойства
Items
Count
TovarName
TovarArticul
IsNotStandart
Методы
FindByName
-->
### [ScItemTovar](#tovar_item_class)
<!--
Свойства
Article
Name
Material
GroupMaterial
TypeElement
ObjList
-->
### [TovarItems]()
### [TScItemTovar]()
### [SalonUtils](salon_utils_obj)
<!--Свойства
PathAttachments
Методы
GetFullPathAttachment
-->

Приложение I.
Создание экранной формы в визуальном режиме . . . . 187
19

# <a name="common_info">Общие сведения</a>  
БАЗИС-скрипты представляют собой ориентированные на прикладного программиста 
инструментальные средства автоматизации проектирования мебели на базе модуля 
БАЗИС-Мебельщик. БАЗИС-скрипты используют синтаксис языка Javascript и 
сохраняются в файлах с расширением js.
## <a name="demo_samples">Демонстрационные примеры БАЗИС-скрипт</a>
В комплект поставки системы БАЗИС включены демонстрационные примеры, 
иллюстрирующие применение скриптов. Используя эти примеры, можно создавать 
собственные скрипты.  
При установке модуля БАЗИС-Мебельщик файлы скриптов автоматически сохраняются в 
папку `<имя системного диска>:\Program Files\BazisSoft\Bazis X\Samples\>`, где X 
представляет собой номер версии.
## <a name="script_editor">Редактор скриптов</a>  
### <a name="launch_editor">Запуск редактора</a>  
Команды работы со скриптами расположены в разделе Скрипты Главного меню 
модуля БАЗИС-Мебельщик. Команда Редактор скриптов позволяет открыть окно 
редактора. Другие команды раздела совпадают с именами файлов скриптов. Если 
щелкнуть левой кнопкой мыши по имени скрипта, он автоматически запустится на 
выполнение. Если выполнить такой щелчок, удерживая нажатой клавишу 
<kbd>Ctrl</kbd>, будет раскрыто окно Редактор скриптов, в котором будет показан
текст скрипта (рис. 1).
### <a name="script_editor_interface">Интерфейс Редактора скриптов</a>
#### <a name="script_editor_menu">Команды редактора</a>
Команды главного меню являются стандартными и позволяют выполнять операции с 
файлами скриптов, а также закрыть окно редактора. Несколько скриптов могут быть 
открыты в редакторе одновременно. Их тексты располагаются на вкладках окна. 
Одна из вкладок является активной. Именно к скрипту, текст которого находится 
на этой вкладке, применяются команды редактора. Команда Запуск заускает 
активный скрипт на выполнение.
#### <a name="script_editor_tab">Вкладка скрипта</a>
Редактор скриптов представляет собой текстовый редактор. Синтаксис команд скрипта 
подсвечивается.
> Текст скрипта можно подготовить в любом стороннем текстовом редакторе.
# <a name="user_interface">Организация взаимодействия с пользователем</a>
Взаимодействие пользователя с программой может выполняться с использованием 
следующих способов:  
- элементы управления (кнопки, поля ввода и т.п.), расположенные на панели 
инструментов,
- элементы управления, расположенные на вспомогательной панели **Свойства**,
- выдача пользователю сообщений, в том числе, требующих его реакции.  

Для простых команд, у которых количество параметров невелико, целесообразно 
располагать элементы управления на панели инструментов. В качестве аналога можно 
привести стандартные команды системы БАЗИС, например, команды группы **Операции**. 
При этом для ускорения доступа к ним автоматически назначаются «горячие клавиши»:
- для доступа к кнопкам <kbd>Shift</kbd>+<kbd>1</kbd>, <kbd>Shift</kbd>+
<kbd>2</kbd> и т.д.
- для доступа к полям ввода <kbd>Alt</kbd>+<kbd>1</kbd>, <kbd>Alt</kbd>+
<kbd>2</kbd> и т.д.  

При создании сложных скриптов, предназначенных для построения параметрических 
моделей, целесообразно размещать элементы управления на вспомогательной панели 
**Свойства**. Это позволяет групировать их, в том числе и
на нескольких уровнях.
## <a name="dynamic_controls"> Элементы управления на панелях инструментов</a>
Чтобы сформировать элементы управления на панелях инструментов, следует
использовать следующие методы:
- NewButtonInput
- NewFloatInput
- NewNumberInput
- NewMaterialInput
- NewButtMaterialInput
- NewFurnitureInput  

## <a name="property_controls">Элементы управления вспомогательной панели Свойства</a>
Чтобы использовать элементы управления вспомогательной панели **Свойства**, 
следует использовать следующие методы и свойства объекта Action.Properties:
- NewGroup – Создать вложенную группу свойств.
- NewImage – Создать вложенную группу свойств c рисунком.
- NewString – Создать свойство типа Строка.
- NewBool – Создать свойство типа Да/Нет.
- NewNumber – Создать свойство типа Число.
- NewButton – Создать свойство с кнопкой редактирования.
- NewMaterial – Создать свойство типа Материал.
- NewButt – Создать свойство типа Материал кромки.
- NewFurniture – Создать свойство типа Фурнитура.
- NewColor – Создать свойство типа Цвет.
- NewSeparator – Создать разделитель.
- PopupMenu – Всплывающее меню.
- DropDownMenu – Выпадающее меню.

## <a name="user_messages">Выдача сообщений пользователю</a>
Выдача пользователю сообщений обеспечивается использованием следующих методов:
- alert – Вывести на экран сообщение или значения параметров.
- confirm – Вывести на экран диалог подтверждения или отмены.
- Hint – Установить строку подсказки.
- ErrorHint –Установить сообщение об ошибке.

# <a name="language_syntax">Синтаксис языка</a>
Синтаксис языка скриптов похож на C++ и Java. Но в любом языке программирования 
присутствует своя специфика представления ключевых и зарезервированных слов, 
составляющих ядро для программирования на этом языке. Ключевые слова всегда 
доступны программисту, но для их использования нужно придерживаться правильного 
синтаксиса.
## <a name="keywords">Список ключевых слов языка программирования БАЗИС)Script:</a>
- break
- switch
- for
- typeof
- continue
- try
- new
- while
- const
- finally
- case
- this
- return
- throw
- in
- default
- var
- else
- if
- catch
- do
- function
- with

## <a name="reserved_words">Список зарезервированных слов:</a>
- boolean
- double
- goto
- interface
- byte
- enum
- implements
- long
- char
- export
- import
- native
- throws
- float
- int
- short

## <a name="comments">Комментарии</a>
К комментариям относится часть кода скрипта, которая никогда не будет выполняться 
программой, однако она очень полезна при дальнейшей разработке. Например, 
используя комментарии, легко можно найти участок созданной ранее программы или 
предоставить возможность другим пользователям сделать это. Комментарии могут 
начинаться с символов <//>, либо вы можете закомментировать участок кода, начав 
с символа открытия комментария </*> и закрыв, соответственно, символом <*/>.  
Примеры:
```js
box(0,0,0,100,100,100,"box1"); //построение параллелепипеда. Все что написано после знака <//> и есть комментарий к коду
/*
Этот участок кода никогда не будет исполнен, он нужен лишь для того, чтобы
в дальнейшем понять, что делалось в данном скрипте, а может быть для от
ладки участка программы...
*/
```
Весь участок кода начиная с символа </*> и заканчивая <*/> игнорируется 
программой и является комментарием
## <a name="variables">Переменные</a>
Для создания переменной используется ключевое слово var.
Примеры:
```js
var x; //создаю переменную x без инициализации
var x = 100; //создаю переменную x, равную 100 целого типа, возможные значения от -2147483648 до 2147483647.
var x, y = 100; //создаю сразу несколько переменных
var x = new Array(4); //создаю массив с 4 элементами(x[0],x[1],x[2],x[3])
var x = "Текст для вывода на экран\nНа второй строке информация\nНа третьей строке..."; //создаю переменную с текстовым содержанием
var x = true; //создаю переменную логического содержания true(истина) или false(ложь)
var x = 1516.2298; //создаю переменную вещественного типа, возможные значения от -1.17549435Е-38 до 3.40282347Е+38.
```
> Внимание! Для корректной работы скриптов имена переменных должны начинаться со 
> строчной или заглавной латинской буквы или знака подчеркивания; имя не должно 
> содержать никаких специальных символов, например: !, ?,| и т.д.; имя не должно 
> совпадать с ключевыми словами языка. Если вы некорректно зададите имя переменной, 
> то при выполнении скрипта будет выведено сообщение об ошибке и ее описание.

При задании текстовой переменной можно использовать спецсимволы, приведенные в 
табл. 1.
Табл.1.

|Символ | Описание                               |
|:----- |----------------------------------------|
|**\b** |Возврат на один символ с его удалением  |
|**\t** | Горизонтальная табуляция               |
|**\n** | Новая строка                           |
|**\v** | Вертикальная табуляция                 |
|**\r** | Возврат каретки                        |
|**\”** | Двойная кавычка                        |
|**\’** | Одинарная кавычка                      |
|**\\** | Обратная косая черта                   |


## <a name="constants">Константы</a>
Для создания констант используется ключевое слово const. Отличием констант 
является то, что их значение нельзя изменить. Основным преимуществом таких типов 
является меньшее количество байт, занятых этими переменными и, как следствие, 
ускорение выполнения кода при использовании const где это возможно.  
**Примеры:**
```js
const message = "Неизменяемый текст"; //создаю константу текстового типа
```
**Арифметические операции**
- Сложение. Пример `x+y`
- Вычитание. Пример `x"y`
- Умножение. Пример `x*y`
- Деление. Пример `x/y`
- Остаток от деления. Пример: `х % у`

Для простоты использования в языке скриптов можно использовать сокращенные записи 
этих операций (табл. 2).  
**Табл.2.**

|Операция   |Описание|
|-----------|--------|
|**x += y** | Сокращенная запись x = x + y|
|**x )= y** | Сокращенная запись x = x " y|
|**x *= y** | Сокращенная запись x = x * y|
|**х /= у** | Сокращенная запись x = x / y|
|**х %= у** | Сокращенная запись x = x % y|
|**++x**    | Сокращенная запись x = x + 1. Увеличение на 1 до присваивания|
|**))x**    | Сокращенная запись x = x " 1. Уменьшение на 1 до присваивания|
|**x++**    | Сокращенная запись x = x + 1. Увеличение на 1 после присваивания|
|**x))**    | Сокращенная запись x = x " 1. Уменьшение на 1 после присваивания|



**Примеры:**
```js
var i = 0;
var a = ++i; //В этом примере переменная i будет сначала увеличена на единицу, а затем переменной a будет присвоен результат. Итог: a = 1.
``` 
```js
var i = 0;
var a = i++; //В этом примере значение переменной i сначала будет присвоено переменной a и только после увеличено на 1. Итог: a = 0.
```
## <a name="logical_ops"> Логические операции</a>
- Логическое "И" " &&
- Логическое "ИЛИ" " ||
**Примеры:**
```js
var i = 0;
var f = 5;
if (f>i && f!=0) {} //Итог: true, т.к. первое и второе условие  true
var i = 10;
var f = 15;
if (i==f || f==0) {} //Итог: false, т.к. ни первое, ни второе условие неверно.
```
## <a name="compare_ops">Операции сравнения</a>
Такие операции необходимы для сравнения одной переменной или константы с другой. 
В табл. 3 приведен список всех возможных операций сравнения:  
**Табл.3.**

|Операция | Описание|
|---------|------------|
|**x == y** | Возвращает true, если x и y равны между собой|
|**x != y** | Возвращает true, если x и y не равны между собой|
|**x === y**| Возвращает true, если x и y равны между собой и их типы совпадают|
|**х < у**  | Возвращает true, если x меньше чем y|
|**х <= у** | Возвращает true, если x меньше или равен y|
|**х > у**  | Возвращает true, если x больше чем y|
|**х >= у** | Возвращает true, если x больше или равен y|

**Примеры:**
```js
true==1 // Итог: true (true преобразуется в 1)
true===1 // Итог: false (true не преобразуется в 1)
5 <= "5" // Итог: true (строка "5" преобразуется в число)
5 === "5" // Итог: false (строка "5" не преобразуется в число)
5 > 4 // Итог: true (5 больше 4)
```
## <a name="if_else">Оператор if...else</a>
Принцип действия следующий: сначала проверяется условие if и если оно верно, то 
выполняется следующий код, а если нет, то выполняется код в записи else, если 
он указан
**Примеры:**
```js
if (10 > 5)
{
//Здесь выполняем код, если условие верно
}
else
{
//Здесь выполняем код, если условие не сработало
}
if (10 < 11)
{
//Здесь выполняем код, если условие верно
} //Оператор else пропущен, следовательно если условие не сработает, то никакой код выполняться не будет
```
## <a name="switch">Оператор switch</a>
Делается выбор по заданному значению. Эта функцию является заменой операторов 
if ... else и является более удобной, когда требуется перебрать множество 
значений
**Пример:**
```js
var num = 10;
switch (num)
{
case 1:
//Выполняем код, если num == 1
break;
case 2:
//Выполняем код, если num == 2
break;
case 100:
//Выполняем код, если num == 100
break;
default:
//Выполняем код, если значение найдено не было
}
```
## <a name="conditional_op">Оператор условного выражения</a>
Очень компактная и удобная функция для выбора одного из двух доступных значений. 
Принцип работы:  
результат = (условие) ? значение1(если условие верно) : значение2(если 
условие не сработало)
**Пример:**
```js
var S = (1 > 0) ? 1500 : 1600; //Соответственно в этом выражении S = 1500, так как условие верно
```
## <a name="break_continue">Операторы break и continue</a>
- break – Команда используется внутри цикла для принудительного прекращения 
выполнения цикла.
- continue – Пропустить невыполненную часть цикла и продолжить выполнения цикла 
со следующими значениями.

**Пример:**
```js 
var S = "Имя_объекта1";
var FindedName = "";
for (var i = 0; i < 10; ++i)
{
    var tested = "Имя_объекта" + i;
    if (tested != S) continue; //Продолжаю поиск со следующими значениями
    else{
        FindedName = tested;
        break; //Принудительно прекращаю поиск, потому как имя объекта уже найдено и цикл больше не нужен
    }
}
if (FindedName != "")
    infomsg("Нашли объект по имени: " + FindedName);
else
    warning("Объект не найден");
```
## <a name="for_cycle">Цикл for</a>
Принцип действия:
for ( имя_переменной и ее стартовое значение; максимальное значение переменной; 
изменение переменной)  
{  
//Тело цикла  
}  
**Пример:**
```js
var num = 0;
for (var i = 0; i < 10; ++i)
{
num += i; //При каждом прохождении цикла значение num увеличивается на величину i
}
history(num); //Поместить результат в историю команд
//Несложно догадаться, что после выполнения такого кода программы num = 45 (0 + 1 + 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9 = 45).
```
## <a name="while_cycle">Цикл while</a>
Аналог оператора организации цикла For; При использовании while нет 
инициализации переменной и ее изменения.
Принцип действия:
while ( условие )
{
//Тело цикла
}
**Пример:**
```js
//Предыдущий пример с оператором for можно записать следующим образом:
var num = 0, i = 0; //Инициализация переменной i в отличии от цикла For происходит заранее
while (i < 10)
{
    num += i; //При каждом прохождении цикла значение num увеличивается на величину i
    ++i; //В отличии от цикла For изменяем значение переменной i в теле цикла
}
history(num); //Результат как и в предыдущем примере num = 45
```
## <a name="do_while_cycle">Цикл do...while</a>
Одна из разновидностей цикла while. Разница состоит в том, что независимо от 
условия while цикл выполнится хотя бы один раз.
Принцип действия:
do
{
//Тело цикла
} while ( условие )
**Пример:**
```js 
//Предыдущий пример с оператором for можно записать следующим образом:
var num = 0, i = 0; //Инициализация переменной i в отличии от цикла For происходит заранее
do
{
    num += i; //При каждом прохождении цикла значение num увеличивается на величину i
    ++i; //В отличии от цикла For изменяем значение переменной i в теле цикла
} while (i < 10)
history(num); //Результат как и в предыдущем примере num = 45
```
## <a name="with_op">Оператор with</a>
Необходим при неоднократном обращении к одному и тому же объекту.
Пример:
```js
//Без оператора with:
history(Math.PI);
history(Math.abs(2));
history(Math.max(4, 10, 7, 6));
//С оператором with:
with(Math)
{
    history(PI);
    history(abs(2));
    history(max(4, 10, 7, 6));
}
```
## <a name="exception_handling">Оператор try...catch...throw</a>
Перехват ошибок выполнения кода программы.
**Пример:**
```js
try
{
    //Участок программы, который может привести к ошибке выполнения
    var S = 100;
    if (S > 99)
        throw ("Значение S слишком большое: " + S); //Сделать выброс
    //Здесь можно продолжить выполнение программы
}
catch (...)
{
    //Этот код будет выполнен в случае возникновения ошибки
    critical(e); //Выводим сообщение об ошибке
}
finally
{
    //Код выполняется в любом случае
    infomsg("Завершили выполнение программы");
}
```
## <a name="functions">Функции</a>
Создание собственных функций в файле скрипта
Принцип действия:
function NameOfFunc(arg1,arg2...argn)
{
//Код функции
return 0; //Возвращаемое значение 0 или любое другое значение
}
**Пример:**
```js
function helloUser(name)
{
infomsg("Доброго времени суток, "+name)
}
var name = GetPar("Ваше имя");
helloUser(name);
```
Вы можете создавать функцию без параметров, а в случае необходимости передать 
ей параметры и узнать их значение при помощи объекта arguments внутри функции.
**Пример:**
```js
function multiply() //Функция перемножения
{
var result = 1;
for (var i = 0; i < arguments.length; ++i)
result *= arguments[i]; //Перемножаю аргументы между собой
return result;
}
infomsg("Результат перемножения 2,3,5,7: " + multiply(2,3,5,7));
```
# <a name="common_variables">Общее для всех модулей</a>
## <a name="global_consts">Глобальные константы</a>
### AxisX
Объект, состоящий из трех свойств:
- x = 1
- y = 0
- z = 0
### AxisY
Объект, состоящий из трех свойств:
- x = 0
- y = 1
- z = 0
### AxisZ
Объект, состоящий из трех свойств:
- x = 0
- y = 0
- z = 1
### Axis_X
Объект, состоящий из трех свойств:
- x = -1
- y = 0
- z = 0
### Axis_Y
Объект, состоящий из трех свойств:
- x = 0
- y = -1
- z = 0
### Axis_Z
Объект, состоящий из трех свойств:
- x = 0
- y = 0
- z = -1

### <a name="view_projections">Направления обзора</a>. Совпадают с основными видами.

|Название | Описание| Числовое значение|
|---------|---------|------------------|
|**p3dFront**| Вид спереди.| 1|
|**p3dBack**| Вид сзади.|2|
|**p3dLeft**| Вид слева.|3|
|**p3dRight**| Вид справа.|4|
|**p3dTop**| Вид сверху.|5|
|**p3dBottom**| Вид снизу.|6|
|**p3dIsometric**| Аксонометрия.|7|

## <a name="global_enums">Глобальные перечисляемые типы</a>
### **<a name="salon_anim_type_enum">SalonAnimationType</a>**
Типы анимации сборок.  

|Значение | Описание|
|--------|----------|
|**None**| Не учитывается в салоне.|
|**Custom**| Учитывается в салоне, не имеет анимации.|
|**DoorLeft**| Дверь левая.|
|**DoorRight**| Дверь правая.|
|**DoorFlap**| Дверь откидная.|
|**DoorLift**| Дверь подъемная.|
|**SDoorLeft**| Дверь купе левая.|
|**SDoorRight**| Дверь купе правая.|
|**Drawer**| Ящик.|
|**Support**| Опора.|
|**Handle**| Ручка.|
|**Facade**| Фасад.|

### **<a name="texture_direction">TextureDir</a>**
Ориентация текстуры пластика панели.  

|Значение|Описание|
|--------|--------|
|**None**| Отсутствует.|
|**Horizontal**| Горизонтальная.|
|**Vertical**| Вертикальная.|

### **<a name="window_position">WindowPosition</a>**
Позиция формы.  

|Значение| Описание|
|--------|--------|
|**Default**| Стандартная позиция формы.|
|**Left**| Форма пристыковывается слева|
|**Right**| Форма пристыковывается справа|

### **<a name="furn_scheme_type">FurnSchemeType</a>**
Тип схемы расстановки крепежа  

|Значение|Описание|
|--------|--------|
|**WithBase**| Тип схемы с фиксированным отступом.|
|**Symmetric**| Симметричный тип схемы.|
|**VariableStep**| Тип схемы с переменным шагом|

### **<a name="model_inspector_error_type">ErrorType</a>**
Тип ошибки анализа модели  

|Значение|Описание|
|--------|--------|
|**ObjIntersection**| Пересечение объектов|
|**FastIntersection**| Пересечение фурнитуры|
|**FastIncorrect**| Неправильная установка фурнитуры|
|**MatNotExists**| Материала нет в наличии|
|**MatOutOfStock**| Материал отсутствует на складе|
|**PanelTooLarge**| Панель невозможно разместить на плите|
|**PlasticTooLarge**| Пластик невозможно разместить на панели|
|**PanelNotFixed**| Панель не закреплена|

### **<a name="furn_datum_mode">DatumMode</a>**
Тип монтирования фурнитуры/фрагмента.  

|Значение|Описание|
|--------|--------|
|**None**| Отсутствует|
|**Face**| На плоскость|
|**FaceFace**| По двум непараллельным плоскостям|
|**FaceButt**| По плоскости и середине торца панели|
|**FaceEdge**| По плоскости и ребру|
|**ParallelFaces**| На 2 параллельные плоскости|
|**Box**| Секция|
|**Scheme**| Крепеж по схеме|

### **<a name="furn_scheme_position">FurniturePosition</a>**
Позиция фурнитуры при установке крепежа по схеме.  

|Значение|Описание|
|--------|--------|
|**Inside**| Установка фурнитуры внутри стыка|
|**Outside**| Установка фурнитуры снаружи стыка|
|**Up**| Установка фурнитуры вверху стыка (только для стыков с горизонтальной панелью)|
|**Down**| Установка фурнитуры внизу стыка (только для стыков с горизонтальной панелью)|

### **<a name="element_type_2d">ElementType</a>**
Тип 2D элемента  

|Значение|Описание|
|--------|--------|
|**Unknown**| Неизвестный|
|**Line**| Линия|
|**Arc**| Дуга|
|**Circle**| Окружность|
|**List**| Список элементов|
|**Ellipse**| Эллипс|

### **<a name="furn_position_mode">FurnPositionMode</a>**
Режим расстановки позиций  

|Значение|Описание|
|--------|--------|
|**All**| Раставить позиции заново|
|**New**| Раставить позиции у новых объектов|
|**Check**| Проверить позиции|

## <a name="global_props">Глобальные свойства</a>
### **system**
Системные функции
Тип: [System](#system_class)

### **Model**
Структура модели
Тип: [Model3D](#model3d_class)

### **Action**
Активный скрипт
Тип: [Action3D](#action3d_class)

### **ActiveMaterial**
Текущий материал
Тип: [FurnMaterial](#furn_mat_class)

### **AnimationType**
Типы анимации сборок и блоков
Тип: [SalonAnimationType](#salon_anim_type_enum)

## <a name="global_methods">Глобальные методы</a>
### **prompt(text)**
Ввод текстового параметра в диалоге.  
Параметры:
- text - подсказка, отображаемая в строке состояния - тип **string**
Возвращает введенное пользователем значение - тип **string**

### **alert(message)**
Вывести на экран сообщение
Параметры:
- message - сообщение - тип **string**

### **confirm(question)**
Вывести на экран диалог подтверждения
Параметры:
- question - текст запроса - тип **string**
Возвращает выбор пользователя - тип **boolean**

### **OpenFurniture(filename)**
Открыть файл фурнитурного изделия для установки в модель.
Параметры:
- filename - путь к файлу - тип **string**
Возвращает объект, содержащий информацию о фурнитуре - тип **InfFurniture**

### **SelectAll()**
Выделить все объекты.

### **UnSelectAll()**
Снять выделение со всех объектов.

### **ViewAll()**
Показать все. Устанавливает масштаб отображения модели, при котором в окне 
редактирования видны все объекты

### **SetCamera(projection)**
Установить направление обзора.
Параметры:
- projection - вид - тип **number**, или [константы направления обзора](#view_projections).

### **GetPoint(hint)**
Запрос точки.
Параметры:
- hint - подсказка запроса, отображаемая в строке состояния - тип **string**
Возвращает указанную пользователем точку - тип [Vector](#vector_class)

### **GetObject(hint)**
Запрос объекта модели.
Параметры:
- hint - подсказка запроса, отображаемая в строке состояния - тип **string**
Возвращает указанный пользователем объект - тип [Object3](#object3_class)

### **GetPanel(hint)**
Запрос панели.
Параметры:
- hint - подсказка запроса, отображаемая в строке состояния - тип **string**
Возвращает указанную пользователем панель - тип [Panel](#panel_class)

### **GetEdge(hint, axis?)**
Запрос выбора ребра, параллельного указанному вектору.
Параметры:
- hint - подсказка запроса, отображаемая в строке состояния - тип **string**
- axis - вектор, параллельно которому должно быть ребро - тип **[Vector](#vector_class)**
Возвращает указанное пользователем ребро - тип [Edge3](#edge3_class)

### **AddPanel(width, height)**
Добавить панель. Панель располагается в плоскости, которая находится ближе других
к плоскости, параллельной экрану. Вершина панели находится в начале координат.
Параметры:
- width - Ширина панели - тип **number**
- height - Высота панели - тип **number**
Возвращает созданную панель - тип [Panel](#panel_class)

### **AddFrontPanel(x1, y1, x2, y2, z)**
Добавить фронтальную панель.
Параметры:
- x1, y1 - координаты начальной точки - тип **number**
- x2, y2 - координаты конечной точки - тип **number**
- z - расстояние от начала координат до панели по оси Z - тип **number**
Возвращает созданную панель - тип [Panel](#panel_class)

### **AddHorizPanel(x1, z1, x2, z2, y)**
Добавить горизонтальную панель.
Параметры:
- x1, z1 - координаты начальной точки - тип **number**
- x2, z2 - координаты конечной точки - тип **number**
- y - расстояние от начала координат до панели по оси Y - тип **number**
Возвращает созданную панель - тип [Panel](#panel_class)

### **AddVertPanel(z1, y1, z2, y2, x)**
Добавить вертикальную панель.
Параметры:
- z1, y1 - координаты начальной точки - тип **number**
- z2, y2 - координаты конечной точки - тип **number**
- x - расстояние от начала координат до панели по оси X - тип **number**
Возвращает созданную панель - тип [Panel](#panel_class)

### **AddExtrusion(name)**
Добавить тело выдавливания.
Параметры:
- name - Имя объекта - тип **string**
Возвращает созданный объект - тип [Extrusion](#extrusion_class)

### **AddTrajectory(name)**
Добавить кинематический элемент (тело по траектории). Траектория представляет 
собой тело, получаемое в результате перемещения контура профиля вдоль контура
траектории. После выполнения команды в модель добавляется пустая траектория. 
Необходимо задать форму контура и траекторию перемещения контура.
Параметры:
- name - Имя объекта - тип **string**
Возвращает созданный объект - тип [Trajectory2D](#trajectory_class)

### **AddBlock(name)**
Добавить блок.
Параметры:
- name - Имя объекта - тип **string**
Возвращает созданный объект - тип [Block](#block_class)

### **AddAssembly(name)**
Добавить сборку.
Параметры:
- name - Имя объекта - тип **string**
Возвращает созданный объект - тип [Block](#block_class)
<!--
### **AddDraftBlock(name)**
Создать полуфабрикат.
Параметры:
- name - Имя объекта - тип **string**
Возвращает созданный объект - тип [Block](#block_class)
-->

### **AddCopy(obj)**
Создать копию объекта.
Параметры:
- obj - Копируемый объект - тип **[Object3](#object3_class)**
Возвращает копию переданного объекта - тип [Object3](#object3_class)

### **DeleteNewObjects()**
Удалить объекты, ранее созданные в скрипте

### **DeleteObject(obj)**
Удалить объект из модели.
Параметры:
- obj - Удаляемый объект - тип **[Object3](#object3_class)**

### **StartEditing(obj)**
Начать редактирование объекта, находящегося в модели. Необходимо вызывать 
команду, чтобы изменения, внесенные в модель в процессе редактирования, могли 
быть отменены командой **Отменить**(<kbd>Ctrl</kbd>+<kbd>z</kbd>).
Параметры:
- obj - Редактируемый объект - тип **[Object3](#object3_class)**

### **BeginBlock(name)**
Начать создание блока. Все объекты, создаваемые после этой команды и до команды 
**EndBlock** попадают внутрь блока.
Параметры:
- name - Имя объекта - тип **string**
Возвращает созданный объект - тип [Block](#block_class)

### **EndBlock()**
Завершить создание блока. Все объекты, создаваемые после команды
BeginBlock и до EndBlock попадают внутрь блока.

### **NewButtonInput(name)**
Создание кнопки на Панели параметров.  
Параметры:
- name - Надпись на кнопке - тип **string**
Возвращает созданный элемент - тип [InButton](#inbutton_class)

### **NewFloatInput(name)**
Создание элемнта на Панели параметров для ввода действительного числа  
Параметры:
- name - Поясняющая надпись - тип **string**
Возвращает созданный элемент - тип [InFloat](#infloat_class)

### **NewNumberInput(name)**
Создание элемнта на Панели параметров для ввода целого числа  
Параметры:
- name - Поясняющая надпись - тип **string**
Возвращает созданный элемент - тип [InNumber](#innumber_class)

### **NewMaterialInput(name)**
Создание элемнта на Панели параметров для выбора материала  
Параметры:
- name - Поясняющая надпись - тип **string**
Возвращает созданный элемент - тип [InMaterial](#inmaterial_class)

### **NewButtMaterialInput(name)**
Создание элемнта на Панели параметров для выбора материала кромки  
Параметры:
- name - Поясняющая надпись - тип **string**
Возвращает созданный элемент - тип [InButtMaterial](#inbuttmaterial_class)

### **NewFurnitureInput(name)**
Создание элемнта на Панели параметров для выбора фурнитуры  
Параметры:
- name - Поясняющая надпись - тип **string**
Возвращает созданный элемент - тип [InFurniture](#infurniture_class)

### **FormatMatName(matName)**
Форматировать имя материала.  
Параметры:
- matName - Полное имя материала в формате `<имя>/n<артикул>` - тип **string**
Возвращает имя материала в формате `<имя>(Артикул <артикул>)` - тип **string**

### **OrientCamera(newDir)**
Повернуть камеру.  
Параметры:
- newDir - Новое направление взгляда камеры - тип **[Vector](#vector_class)**

### **ExtractMatName(matName)**
Извлечь имя материала из полного имени.  
Параметры:
- matName - Полное имя материала в формате `<имя>/n<артикул>` - тип **string**
Возвращает только имя материала - тип **string**

### **ExtractMatCode(matName)**
Извлечь артикул материала из полного имени
Параметры:
- matName - Полное имя материала в формате `<имя>/n<артикул>` - тип **string**
Возвращает только артикул материала - тип **string**

# <a name="common_types">Общие типы для всех модулей</a>
## <a name="geometry2d_class">Geometry2D</a>
Тип системного объекта для реализации вспомогательных геометрических алгоритмов.  
**Методы:**
### Intersect(elem1, elem2)
Вычислить точки пересечения двухмерных элементов.  
Параметры:
- elem1, elem2 - пересекающиеся двухмерные элементы - тип **[Elem2D](#elem2d_class)**  

Возвращает массив найденных точек пересечения - тип **Array<[Point](#point_class)>**  

### **Compare(elem1, elem2)**
Сравнить элементы.  
Параметры:
- elem1, elem2 - сравниваемые двухмерные элементы - тип **[Elem2D](#elem2d_class)**  

Возвращает результат сравнения - тип **boolean**  

### **Distance(elem1, elem2)**
Найти кратчайшее расстояние между элементами.  
Параметры:
- elem1, elem2 - двухмерные элементы - тип **[Elem2D](#elem2d_class)**  

Возвращает расстояние между элементами - тип **number**  

### **Area(contour)**
Найти площадь контура.  
Параметры:
- contour - двухмерный контур - тип **[Contour2D](#contour2d_class)**

## <a name="system_class">System</a>
Тип системного объекта

## **Свойства:**
### **apiVersion**
Текущая версия Bazis API - тип **number**

## **Методы:**
### **include(file)**
Подключить указанный файл JavaScript. Подключение осуществляется путем 
выполнения кода из файла.  
Параметры:
- file - Имя подключаемого файла - тип **string**

### **log(msg)**
Вывести диагностическое сообщение в лог.  
Параметры:
- msg - Текст сообщения - тип **string**

### **fileExists(file)**
Проверить, существует ли указанный файл
Параметры:
- file - Имя файла - тип **string**  

Возвращает результат проверки - тип **boolean**

### **writeTextFile(file, content)**
Записать текст в файл.  
Параметры:
- file - Имя файла - тип **string**
- content - Содержимое файла - тип **string**

### **askWriteTextFile(ext, content)**
Записать текст в файл с запросом имени файла в диалоговом окне  
Параметры:
- ext - Расширение файла - тип **string**
- content - Содержимое файла - тип **string**

### **readTextFile(file)**
Считать текст из файла  
- file - Имя файла - тип **string**;

Возвращает содержимое файла - тип **string**

### **askReadTextFile(ext)**
Считать текст из файла с запросом выбора файла в диалоговом окне  
Параметры:
- ext - Расширение файла - тип **string**  

Возвращает содержимое файла - тип **string**

### **secureExec(str)**
Выполнить зашифрованный код.  
> Метод позволяет выполнить зашифрованный скрипт. Шифровать текст текущего 
> скрипта позволяет команда Редактора скриптов **Правка** –> **Шифрование кода**. 
> Перед выполнением команды следует выделить текст скрипта, который необходимо 
> зашифровать. Если не выделено ничего, шифруется скрипт целиком. После вызова 
> команды на экране появится диалог **Шифрование кода**. В этом диалоге можно 
> ввести номер ключа аппаратной защиты системы БАЗИС. Скрипт, «привязанный» таким 
> образом к ключу, может быть выполнен только в модуле БАЗИС-Мебельщик, защищенном 
> этим ключом. Если номер не задан (номер ключа = 0), привязка отсутствует, скрипт 
> может быть выполнен в любом модуле БАЗИС"Мебельщик. Можно ввести несколько 
> номеров ключей, разделяя их знаком `;`.  
Параметры:
- str - зашифрованный код - тип **string**;

### **exec(str, params)**
Выполнить внешнюю программу.  
Параметры:
- str - полное имя исполняемого файла - тип **string**
- params - Параметры для исполняемого файла - тип **string**

### **getFileName(filename)**
Получить имя файла без пути.  
Параметры:
- filename - полное имя файла - тип **string**  

Возвращает имя файла без пути - тип **string**

### **getFileNameWithoutExtension(filename)**
Получить имя файла без пути и расширения.  
Параметры:
- filename - полное имя файла - тип **string**  

Возвращает имя файла без пути и расширения - тип **string**

### **askFileNameSave(ext)**
Открыть диалоговое окно сохранения файла.  
Параметры:
- ext - расширение файла - тип **string**  

Возвращает полное имя выбранного файла - тип **string**

### **askFolder(caption, default)**
Открыть диалоговое окно выбора папки.  
Параметры:
- caption - заголовок окна - тип **string**  
- default - папка по умолчанию - тип **string**

Возвращает выбранную пользователем папку - тип **string**

## <a name="model3d_class">Model3D</a>
Тип модели. Унаследован от **[List3D](#list3d_class)**.

## **Свойства:**
### **Selected**
Выделенный объект модели. Если выделено несколько объектов, то первый из них. -
тип **[Object3](#object3_class)**

### **SelectionCount**
Количество выделенных элементов. - тип **number**

### **Count**
Количество объектов в модели. - тип **number**

## **Индексные свойства:**
### **Selections[i]**
Параметр **i** - индекс элемента - тип **number**
Возвращает выделенный элемент по индексу **i** - тип **[Object3](#object3_class)**

### **Objects[i]**
Параметр **i** - индекс элемента - тип **number**
Возвращает объект модели по индексу **i** - тип **[Object3](#object3_class)**

## <a name="action3d_class">Action3D</a>
Тип текущего скрипта.

## **Свойства:**
### **Interactive**
Возможность взаимодействия с пользователем. Если равно false, то запрещены 
любые функции взаимодействия с пользователем - тип **boolean**

### **MouseX**
Координата X позиции курсора мыши на экране - тип **[Point](#point_class)**

### **MouseY**
Координата Y позиции курсора мыши на экране - тип **[Point](#point_class)**

### **Pos3**
Текущая позиция курсора в окне модели - тип **[Vector](#vector_class)**

### **ViewDir**
Нормаль к текущему виду (направление взгляда камеры) - тип **[Vector](#vector_class)**

### **UpDir**
Вектор вверх текущего вида. - тип **[Vector](#vector_class)**

### **RightDir**
Вектор вправо текущего вида - тип **[Vector](#vector_class)**

### **ShowPoints**
Разрешать подсвечивать точки - тип **boolean**

### **ShowEdges**
Разрешать подсвечивать ребра - тип **boolean**

### **Hint**
Установить строку подсказки - тип **string**

### **ErrorHint**
Установить сообщение об ошибке - тип **string**

### **BlinkHint**
Установить мигающую подсказку - тип **string**

### **OnClick**
Обработчик щелчка мыши - тип **function**

### **OnMove**
Обработчик перемещения курсора мыши - тип **function**

### **OnStart**
Обработчик начала работы скрипта. Вызывается после загрузки значений 
свойств - тип **function**

### **OnFinish**
Обработчик завершения работы скрипта - тип **function**

### **Properties**
Набор редактируемых свойств - тип **[RootProperties](#root_props_class)**

### **OnRayTraceFinished**
Обработчик завершения тонирования изображения - тип **function**

### **ModelFilename**
Имя файла текущей модели - тип **string**

## **Методы:**
### **Continue()**
Продолжить обработку прерываний после завершения основного тела скрипта, 
не завершая скрипта.

### **Commit()**
Применить изменения в модели внесенные в скрипте, не завершая скрипта.

### **Finish()**
Завершить работу скрипта.

### **Cancel()**
Завершить работу скрипта, отказавшись от изменений.

### **AsyncExec(func)**
Выполнить функцию, в которой доступны запросы Get*.  
Параметры:
- func - функция для выполнения - тип **function**

### **<a name="action_begin_ortho3">BeginOrtho3(point)</a>**
Включить режим ортогональных построений относительно точки.  
> Чтобы отключить режим ортогональных построений, необходимо использовать 
> метод [EndOrtho3](#action_end_ortho3).  

Параметры:
- point - точка - тип **[Vector](#vector_class)**

### <a name="action_end_ortho3">**EndOrtho3()</a>**
Выключить режим ортогональных построений относительно точки (см. метод 
[BeginOrtho3](#action_begin_ortho3))

### **CursorToClosestPoint()**
Сдвинуть курсор к ближайшей точке привязки.

### **CursorToClosestLine()**
Сдвинуть курсор к ближайшей линии.

### **CursorToMiddleOfLine()**
Сдвинуть курсор к ближайшей середине линии.

### **Find3DPoint()**
Найти точку на модели в текущем положении курсора мыши.  
Возвращает найденную точку - тип [Vector](#vector_class)

### **Find3DPointXZPlane()**
Найти точку на плоскости X0Z.  
Возвращает найденную точку - тип [Vector](#vector_class)

### **Get3Dobject()**
Найти объект под курсором мыши.  
Возвращает найденный объект - тип [Object3](#object3_class)

### **RayTraceScene()**
Запустить тонирование изображения.

### **LoadModel(file)**
Загрузить модель из файла.
> **Внимание:** Модель загружается вместо открытой, поэтому рекомендуется 
> сохранить открытую модель перед загрузкой новой.  
Параметры:
- filename - имя файла - тип **string**

### **SaveModel(file)**
Сохранить модель в файл.  
Параметры:
- filename - имя файла - тип **string**

### **NewModel()**
Создать новую модель.
> **Внимание:** Модель создается вместо открытой, поэтому рекомендуется 
> сохранить открытую модель перед загрузкой новой.  

### **NewFurniture()**
Создать новую фурнитуру.
> **Внимание:** Модель создается вместо открытой, поэтому рекомендуется 
> сохранить открытую модель перед загрузкой новой.  

### **NewFragment()**
Создать новый фрагмент.
> **Внимание:** Модель создается вместо открытой, поэтому рекомендуется 
> сохранить открытую модель перед загрузкой новой.  

### **Revert()**
Отменить изменения в модели, внесенные в скрипте.

### **ArrangePositions(mode, model)**
Расставить позиции.  
Параметры:
- mode - режим расстановки - тип [FurnPositionMode](#furn_position_mode)
- model - структурный объект - тип [List3D](#list3d_class)

Возвращает результат успешности раастановки - тип **boolean**

### **ReplaceFurniture(old, new, fasteners)**
Заменить фурнитуру.  
Параметры:
- old - список названий старой фурнитуры - тип **Array<string>**
- new - список значений новой фурнитуры - тип **Array<[InfFurniture](#furniture_info_class)>**
- fasteners - список объектов для замены - тип **Array<[Object3](#object3_class)>**
> **Внимание:** для корректной работы функции, списки старой и новой фурнитуры 
> должны быть одинаковой длины. Каждому элементу списка старой фурнитуры 
> соответствует элемент списка новой фурнитуры с тем же индексом.  

### **ChooseMaterial()**
Вызов окна выбора материала из базы данных материалов.  
Возвращает полное имя выбранного материала, тип **string**.

## <a name="script_prop_class">ScriptProperty</a>
Набор редактируемых свойств.

## **Свойства:**
### **Name**
Имя свойства - тип **string**

### **Enabled**
Возможность изменения свойства пользователем - тип **boolean**

### **ChildrenEnabled**
Доступность вложенных свойств для редактирования - тип **boolean**

### **Visible**
Видимость свойства в панели свойств - тип **boolean**

### **Count**
Количество вложенных свойств первого уровня вложенности - тип **number**

### **Expanded**
Развернуты ли вложенные свойства - тип **boolean**  

### **ValueValid**
Флаг корректности введенного значения, выставляется обработчиком 
**[OnValueValidate](#script_prop_on_validate)** - тип **boolean**

### **NameEditable**
Разрешить редактирование имени - тип **boolean**

### **BackColor**
Цвет фона - тип **number**

### **PopupMenu**
Всплывающее меню - тип **[ScriptMenu](#script_menu_class)**

### **DropDownMenu**
Выпадающее меню - тип **[ScriptMenu](#script_menu_class)**

### **Tag**
Пользовательское число - тип **number**

### **OnChange**
Обработчик изменения свойства и вложенных свойств - тип **function**

### **OnValueChange**
Обработчик изменения значения свойства - тип **function**

### **OnActivate**
Обработчик активации свойства пользователем -тип **function**

### **OnDeactivate**
Обработчик деактивации свойства или меню - тип **function**

### **<a name="script_prop_on_validate">OnValueValidate</a>**
Обработчик проверки корректности значения - тип **function**

## **Индексные свойства**
### **Items[i]**
Параметр **i** - индекс свойства - тип **number**  
Возвращает свойство первого уровня вложенности - тип **[ScriptProperty](#script_prop_class)**

## **Методы:**
### **Clear()**
Очистить вложенные свойства.

### **Save(file)**
Сохранить введенные пользователем значения свойств в файл.  
Параметры:
- file - имя файла - тип **string**

### **Load(file)**
Загрузить значения свойств из файла.  
Параметры:
- file - имя файла - тип **string**

### **NewGroup(name)**
Создать вложенную группу свойств.  
Параметры:
- name - имя группы - тип **string**  

Возвращает созданную группу - тип **[ScriptGroupProperty](#script_group_class)**

### **NewImage(name, file)**
Создать вложенную группу свойств c рисунком.  
Параметры:
- name - имя группы - тип **string**
- file - имя файла рисунка - тип **string**  

Возвращает созданную группу - тип **[ScriptGroupProperty](#script_group_class)**

### **NewString(name, val)**
Создать свойство строкового типа.   
Параметры:
- name - имя свойства - тип **string**
- val - значение свойства - тип **string**  

Возвращает созданное свойство - тип **[ScriptStringProperty](#script_string_class)**

### **NewBool(name, val)**
Создать свойство логического (boolean) типа.  
Параметры:
- name - имя свойства - тип **string**
- val - значение свойства - тип **boolean**  

Возвращает созданное свойство - тип **[ScriptBooleanProperty](#script_bool_class)**

### **NewNumber(name, val)**
Создать свойство числового типа.   
Параметры:
- name - имя свойства - тип **string**
- val - значение свойства - тип **number**  

Возвращает созданное свойство - тип **[ScriptNumberProperty](#script_number_class)**

### **NewButton(name)**
Создать свойство с кнопкой.  
Параметры:
- name - имя свойства - тип **string**  

Возвращает созданное свойство - тип **[ScriptButtonProperty](#script_button_class)**

### **NewMaterial(name)**
Создать свойство типа Материал.  
Параметры:
- name - имя свойства - тип **string**  

Возвращает созданное свойство - тип **[ScriptMaterialProperty](#script_material_class)**

### **NewButt(name)**
Создать свойство типа Материал кромки.  
Параметры:
- name - имя свойства - тип **string**  

Возвращает созданное свойство - тип **[ScriptButtProperty](#script_butt_class)**

### **NewFurniture(name)**
Создать свойство типа Фурнитура.  
Параметры:
- name - имя свойства - тип **string**  

Возвращает созданное свойство - тип **[ScriptFurnitureProperty](#script_furn_class)**

### **NewColor(name)**
Создать свойство типа Цвет.  
Параметры:
- name - имя свойства - тип **string**  

Возвращает созданное свойство - тип **[ScriptMaterialProperty](#script_material_class)**

### **NewSeparator()**
Создать разделитель.  
Возвращает созданное свойство - тип **[ScriptProperty](#script_prop_class)**

### **Validate()**
Проверить значение свойства и вложенных свойств.
Возвращает результат проверки - тип **boolean**

## **<a name="script_group_class">ScriptGroupProperty</a>**
Группа свойств скрипта. Унаследовано от [ScriptProperty](#script_prop_class)  
## **Свойства:**
### **Image**
Путь к файлу изображения для кнопки - тип **string**
### **MaxHeight**
Максимальная высота картинки - тип **number**
### **Scrollable**
Наличие полосы прокрутки - тип **boolean**

## **<a name="script_string_class">ScriptStringProperty</a>**
Строковое свойство. Унаследовано от [ScriptProperty](#script_prop_class)  
## **Свойства:**
### **Value**
Значение свойства - тип **string**

## **<a name="script_bool_class">ScriptBooleanProperty</a>**
Логическое (boolean) свойство. Унаследовано от [ScriptProperty](#script_prop_class)  
## **Свойства:**
### **Value**
Значение свойства - тип **boolean**

## **<a name="script_number_class">ScriptNumberProperty</a>**
Числовое свойство. Унаследовано от [ScriptProperty](#script_prop_class)  
## **Свойства:**
### **Value**
Значение свойства - тип **number**
### **MaxValue**
Максимальное значение свойства - тип **number**
### **MinValue**
Минимальное значение свойства - тип **number**

> Если значение `MinValue` больше значения `MaxValue` у числового свойства 
> появляется ползунок, с помощью которого можно менять значение числового свойства.
> Шаг ползунка определяется значением `ValueStep`
### **ValueStep**
Шаг изменения значения свойства с помощью ползунка - тип **number**

## **<a name="script_button_class">ScriptButtonProperty</a>**
Свойство типа Кнопка. Унаследовано от [ScriptProperty](#script_prop_class)  
## **Свойства:**
### **Value**
Надпись на кнопке - тип **string**
### **OnClick**
Функция"обработчик нажатия на кнопку - тип **function**

## **<a name="script_material_class">ScriptMaterialProperty</a>**
Свойство типа Материал. Унаследовано от [ScriptProperty](#script_prop_class)  
## **Свойства:**
### **Width**
Ширина листа - тип **number**
## **Методы:**
### **SetActive()**
Установить материал активным. Все последующие элементы будут построены из этого 
материала.

## **<a name="script_material_class">ScriptMaterialProperty</a>**
Свойство типа Материал кромки. Унаследовано от [ScriptProperty](#script_prop_class)  
## **Свойства:**
### **Width**
Ширина ленты - тип **number**
### **Thickness**
Толщина кромки - тип **number**
## **Методы:**
### **SetActive()**
Установить материал кромки активным. Все последующие элементы будут построены 
из этого материала.

## **<a name="script_furn_class">ScriptFurnitureProperty</a>**
Свойство типа Фурнитура. Унаследовано от [ScriptProperty](#script_prop_class)  
## **Свойства:**
### **Value**
Значение свойства (фурнитура) - тип **[InfFurniture](#furniture_info_class)**

## **<a name="script_furn_class">ScriptFurnitureProperty</a>**
Свойство типа Цвет
## **Свойства:**
### **Value**
Значение свойства (цвет) - тип **number**

## **<a name="script_furn_class">ScriptFurnitureProperty</a>**
Свойство типа всплывающее или выпадающее меню. Унаследовано от 
[ScriptProperty](#script_prop_class)  
## **Свойства:**
### **Store**
Сохраняется ли свойство в файл - тип **boolean**

## **<a name="script_form_class">ScriptForm</a>
Пользовательская экранная форма, позволяющая задавать параметры объектов.
## **Свойства:**
### **Properties**
Набор редактируемых свойств - тип **[ScriptProperty](#script_prop_class)**
### **Caption**
Заголовок формы - тип **string**
### **Width**
Ширина формы - тип **number**
### **Height**
Высота формы - тип **number**
### **MinWidth**
Минимальная ширина формы - тип **number**
### **MinHeight**
Минимальная высота формы - тип **number**
### **Visible**
Видимость формы - тип **boolean**
### **Left**
Положение левого края формы - тип **number**
### **Top**
Положение верхнего края формы - тип **number**
### **OKButton**
Показывать кнопку `ОК` на форме - тип **boolean**
### **OKButtonCaption**
Текст кнопки `ОК` - тип **string**
### **CancelButton**
Показывать кнопку `Отмена` на форме - тип **boolean**
### **CancelButtonCaption**
Текст кнопки `Отмена` - тип **string**
### **OnClose**
Обработчик закрытия формы - тип **function**
### **OnShow**
Обработчик открытия формы - тип **function**
### **Resizable**
Возможность изменять размеры формы - тип **boolean**
### **Dockable**
Возможность пристыковывать немодальную форму - тип **boolean**
### **OnOkButtonClick**
Обработчик нажатия на кнопку `OK` - тип **function**
### **OnCancelButtonClick**
Обработчик нажатия на кнопку `Отмена` - тип **function**
## **Методы:**
### **Show(windowPos)**
Показать немодальную форму (форма не будет блокировать доступ к другим 
компонентам приложения)  
Параметры:
- windowPos - позиция формы - тип **[WindowPosition](#window_position)**
### **ShowModal()**
Показать модальную форму (форма будет блокировать доступ к другим 
компонентам приложения)  
Возвращает результат вызова в зависимости от нажатия кнопки `ОК` или `Отмена` -
 тип **boolean**
### **Close()**
Закрыть форму.

## **<a name="furn_mat_class">FurnMaterial</a>**
Материал.
## **Свойства:**
### **Name**
Наименование материала - тип **string**
### **Thickness**
Толщина материала - тип **number**
### **Width**
Ширина материала - тип **number**
## **Методы:**
### **Make(name, thickness, width?)**
Создать материал по наименованию и толщине или ширине  
Параметры:  
- name - Имя материала - тип **string**
- thickness - Толщина материала - тип **number**
- width - Ширина материала - тип **number**

## **<a name="vector_class">Vector</a>**
Точка в трехмерном пространстве.
## **Свойства:**
### **x**
координата X точки - тип **number**
### **y**
координата Y точки - тип **number**
### **z**
координата Z точки - тип **number**

## **<a name="point_class">Point</a>**
Точка на плоскости.
## **Свойства:**
### **x**
координата X точки - тип **number**
### **y**
координата Y точки - тип **number**

## **<a name="edge3_class">Edge3</a>**
Ребро.
## **Свойства:**
### **First**
Начало ребра в ЛСК - тип **[Vector](#vector_class)**
### **Last**
Конец ребра в ЛСК - тип **[Vector](#vector_class)**
### **GFirst**
Начало ребра в глобальной системе координат - тип **[Vector](#vector_class)**
### **GLast**
Конец ребра в глобальной системе координат - тип **[Vector](#vector_class)**


## **<a name="object3_class">Object3</a>**
Трехмерный объект.
## **Свойства:**
### **Name**
Наименование - тип **string**
### **ArtPos**
Артикул - тип **string**
### **Owner**
Родитель объекта - тип **[List3D](#list3d_class)**
### **Visible**
Видимость объекта - тип **boolean**
### **Selected**
Является ли объект выделенным - тип **boolean**
### **List**
Является ли объект структурным -  тип **boolean**
### **AsList**
Привести объект к структурному - тип **[List3D](#list3d_class)**
### **AsPanel**
Привести объект к типу панели - тип **[Panel](#panel_class)**
### **Position**
Положение объекта - тип **[Vector](#vector_class)**
### **PositionX**
Координата X - тип **number**
### **PositionY**
Координата Y - тип **number**
### **PositionZ**
Координата Z - тип **number**
### **GMax**
Вершина габаритного параллелепипеда, наиболее удаленная от начала системы 
координат родительского объекта - тип **[Vector](#vector_class)**
### **GMin**
Вершина габаритного параллелепипеда, наименее удаленная от начала системы 
координат родительского объекта - тип **[Vector](#vector_class)**
### **GSize**
Длина диагонали габаритного параллелепипеда объекта, расстояние от `GMax`
до `Gmin` - тип **[Vector](#vector_class)**
### **GabMin**
Вершина габаритного параллелепипеда, наименее удаленная от начала глобальной 
системы координат - тип **[Vector](#vector_class)**
### **GabMax**
Вершина габаритного параллелепипеда, наиболее удаленная от начала глобальной 
системы координат - тип **[Vector](#vector_class)**
### **UserPropCount**
Количество пользовательских свойств - тип **number**

## **Индексные свойства:**
### **UserProperty[index]**
Параметр **index** - индекс или имя пользовательского свойства - тип **number** 
или **string**  
Возвращает значение пользовательского свойства по указанному имени или индексу 
- тип **string**
### **UserPropertyName[i]**
Параметр **i** - индекс пользовательского свойства - тип **number**  
Возвраащет имя пользовательского свойства по указанному индексу - тип **string**

## **Методы:**
### **SetDefaultTransform()**
Установить нулевые положение и ориентацию объекта.
### **Translate(dir)**
Переместить объект в системе координат родителя.  
Параметры:
- dir - Вектор смещения - тип **[Vector](#vector_class)**
### **Rotate(axis, angle)**
Повернуть вокруг заданной оси в СК родительского объекта.  
Параметры:
- axis - ось вращения - тип **[Vector](#vector_class)**
- angle - угол поворота в градусах - тип **number**
### **TranslateGCS(dir)**
Сместить объект в глобальной системе координат.  
Параметры:
- dir - Вектор смещения - тип **[Vector](#vector_class)**
### **RotateGCS(axis, angle)**
Повернуть вокруг заданной оси в глобальной системе координат.  
Параметры:
- axis - ось вращения - тип **[Vector](#vector_class)**
- angle - угол поворота в градусах - тип **number**
### **RotateX(angle)**
Повернуть вокруг оси X.  
Параметры:
- angle - угол поворота в градусах - тип **number**
### **RotateY(angle)**
Повернуть вокруг оси Y.  
Параметры:
- angle - угол поворота в градусах - тип **number**
### **RotateZ(angle)**
Повернуть вокруг оси Z.  
Параметры:
- angle - угол поворота в градусах - тип **number**
### **Orient(axisz, axisy)**
Развернуть объект относительно двух осей.  
Параметры:
- axisz - направление вдоль которого будет направлена ось Z локальной системы 
координат объекта - тип **[Vector](#vector_class)**
- axisy - направление вдоль которого будет направлена ось Y локальной системы 
координат объекта - тип **[Vector](#vector_class)**
### **OrientGCS(axisz, axisy)**
Развернуть объект относительно двух осей в глобальной СК.  
Параметры:
- axisz - направление вдоль которого будет направлена ось Z локальной системы 
координат объекта - тип **[Vector](#vector_class)**
- axisy - направление вдоль которого будет направлена ось Y локальной системы 
координат объекта - тип **[Vector](#vector_class)**
### **Reflect(pos, normal)**
Отразить объект относительно плоскости.  
Параметры:
- pos - точка, через которую проходит плоскость - тип **[Vector](#vector_class)**
- normal - точка, через которую проходит перпендикуляр к плоскости - тип 
**[Vector](#vector_class)**
### **ToObject(pos)**
Преобразовать координаты точки из глобальной СК в ЛСК объекта.  
Параметры:
- pos - точка - тип **[Vector](#vector_class)**  

Возвращает преобразованную точку - тип **[Vector](#vector_class)**
### **ToGlobal(pos)**
Преобразовать координаты точки из ЛСК объекта в глобальную СК.  
Параметры:
- pos - точка - тип **[Vector](#vector_class)**  

Возвращает преобразованную точку - тип **[Vector](#vector_class)**
### **NToObject(normal)**
Преобразовать нормаль из глобальной СК в ЛСК объекта.  
Параметры:
- normal - нормаль - тип **[Vector](#vector_class)**  

Возвращает преобразованную нормаль - тип **[Vector](#vector_class)**
### **NToGlobal(normal)**
Преобразовать нормаль из СК объекта в глобальную СК.  
Параметры:
- normal - нормаль - тип **[Vector](#vector_class)**  

Возвращает преобразованную нормаль - тип **[Vector](#vector_class)**
### **Build()**
Перестроить объект после изменения его свойств.
### **IsOwner(obj)**
Определить, является ли объект obj родителем объекта.  
Параметры:
- obj - предполагаемый родитель объекта - тип **[Object3](#object3_class)**  

Возвращает результат типа **booolean**