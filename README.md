Домашнее задание к занятию «Введение в Java»
Инструкция к выполнению домашнего задания
Перед тем как отправить своё решение на проверку преподавателю, сверьтесь с чеклистом.

1. В решении выполнены все требования задания 🆕
Убедитесь, что все требования задания выполнены. Для этого перед отправкой внимательно прочтите весь текст условия задания и соотнесите сказанное в нём с вашим решением. Навык самопроверки работы перед ревью пригодится вам как при обучении, так и на работе.

2. Проект и репозиторий настроены правильно 🆕
Репозиторий должен быть папкой вашего idea-проекта. Обратите внимание, что репозиторием не должна быть папка, в которой лежит папка проекта, он сам должен быть папкой проекта. В нём должны быть соответствующие файлы и папки — src и другие.

Не забудьте создать .gitignore-файл в корне проекта и добавить туда в игнорирование автогенерируемую папку out и папку настроек идеи .idea.

3. Что делать, если возникли сложности 🆕
Это здорово. Если их преодолевать правильно, то можно получить большую образовательную пользу для себя. Периодическое возникновение вопросов, недопонимание пройденного материала — нормальная и неотъемлемая часть обучения. А мы здесь, чтобы помочь вам пройти этот путь.

Что делать, если непонятна теория
Если подобный вопрос разбирался на лекции, посмотрите ещё раз раздел с этой темой в видеозаписи.
Если вопрос не решился, попробуйте поискать ответ самостоятельно в интернете, этот навык пригодится вам в работе.
Если самостоятельно разобраться не удалось, задайте вопрос в общем чате, мы обязательно поможем.
Что делать, если непонятно условие задания
Прежде чем задать вопрос по условию задачи, перечитайте его ещё раз и убедитесь, что в тексте условия нет прямого ответа на этот вопрос. Умение работать с текстом — важный навык работы с информацией.
Если ответа на свой вопрос в тексте условия не увидели, задайте его в общем чате, мы раскроем детали условия.
Что делать, если не получается задача
Если ваша проблема — это ошибка компиляции — подчёркивает красным, не даёт запустить программу сборки проекта, CI и прочие подобные ошибки, то:

Найдите и прочитайте текст ошибки, который вам подсвечивает идея или логи. «Подчёркивает красным» — это не описание ошибки.
Попробуйте понять текст ошибки, при необходимости воспользуйтесь переводчиком. Не страшно, если вы переведёте неточно, тут главное — сам процесс: со временем и с нашей помощью вы будете это делать лучше и лучше, но, пропуская этот этап, вы не сможете научиться это делать.
Если не получилось понять ошибку по её тексту, попробуйте её загуглить и изучить подобную ошибку у других людей. Попробуйте примерить решения их проблем на свой код. Соотнесите найденные описания ошибки с пройденной теорией.
Если всё равно ваши трудности не разрешились, напишите в общий чат, обязательно указав:
название задачи и ссылку на условие;
ссылку на вашу работу;
текст и скриншот, не фотографию, ошибки;
ваши размышления и описание шагов, которые вы совершили для решения.
Если ваша проблема — это ошибка исполнения, программа умирает уже после запуска, или она отрабатывает неправильно, из-за чего ваши тесты не проходят, то:

Воспользуйтесь отладчиком для пошагового анализа работы вашей программы. Так вы или убедитесь в неправильности придуманного вами алгоритма, или найдёте конкретное место, где ожидаемое поведение программы разошлось с фактическим.
Если проблему найти не получилось, напишите в общий чат, обязательно указав:
название задачи и ссылку на условие;
ссылку на вашу работу;
конкретное и подробное описание проблемы или затруднения при решении задачи. «Помогите, что-то не так» — это не описание;
подробное описание вашего анализа программы с помощью отладчика вместе со скринами;
ваши размышления и описание шагов, которые вы совершили для решения.
Задание. Рецепт
Ваша задача — проанализировать программу расчёта распределения ингредиентов на порцию. Программе на вход даётся рецепт со всеми граммовками каждого ингредиента, а также количество человек, которые будут в одинаковых порциях его есть. На выходе программа указывает без округлений, какое точное количество каждого ингредиента пришлось на одну порцию еды.

public class Main {
    public static void main(String[] args) {

        int eaters = 5; // сколько людей будут есть

        int water = 3000; // миллилитров воды
        int potatoes = 5; // картофелин
        int chicken = 6; // куриных бёдер
        int spices = 10; // ложек специй

        System.out.println("Сварили суп. На одного человека вышло:");
        System.out.println((water / eaters) + " миллилитров воды");
        System.out.println((potatoes / eaters) + " картофелин(а)");
        System.out.println((chicken / eaters) + " куриных(ое) бёдер(ро)");
        System.out.println((spices / eaters) + " ложек(ка) специй");

    }
}
Для анализа этой программы

Установите бесплатную версию идеи (Community version) с официальной страницы.
Создайте новый проект на основе Java 11, идея может скачать её сама, если вы в меню выбора Java выберите Download JDK. Обратите внимание, что в левой части меню следует выбирать New Project, а не что-либо другое.
image

Создайте класс Main с содержимым из кода выше.
Нажмите на кнопку запуска программы. Она должна запуститься, вывести информацию на экран и завершиться.
Закоммитьте и запушьте ваш проект в публичный репозиторий на GitHub.
Проанализируйте код и вывод программы. Найдите в них дефекты. Менять код программы не нужно.
Оформите баг-репорт с помощью GitHub Issues, описывающий найденный дефект по шаблону из примера ниже.
Формат оформления баг-репорта
Наша цель — получить такой баг-репорт:

image

Это можно сделать, написав следующее:

image

Комментарии к формату:

И в .md-файлах, и внутри описания баг-репортов используется формат Markdown.
Исходный код Issue специально вставлен картинкой, чтобы вы вчитывались и перепечатывали, а не копировали.
Чтобы красиво сослаться на нужное место в коде на GitHub (в нашем случае для отображения локации), откройте этот файл на GitHub, нажмите на номер или номера соответствующей строки, удерживая Shift, и рядом слева нажмите на троеточие, в выпавшем меню нажмите Copy permalink. В буфер обмена скопируется прямая ссылка на эту строку этого коммита. Теперь вы её можете просто вставить в текст Issue как в шаблоне:
image

Для загрузки изображений вы можете воспользоваться кнопкой, находящейся сразу под полем редактирования текста. Также возможна автозагрузка скриншотов прямо из буфера обмена через Ctrl+V с автовставкой в место нахождения курсора:
image

Результат
При отправке решения в личном кабинете прикрепите ссылку на ваш публичный репозиторий GitHub.
