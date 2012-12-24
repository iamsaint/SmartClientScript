# SmartClientScript

Расширение стандартного компонента ClientScript фреймворка Yii.

## Возможности

1.  Добавлена новая константа SmartClientScript::POS\_HEAD\_BEGIN. Она позволяет регистрировать скрипты в секции HEAD до cкриптов с SmartClientScript::POS_HEAD. Таким образом появляется возможность разместить в секции HEAD фрагменты Javascript кода до объявления JS файлов. В стандартном ClientScript такой возможности нет.

2.  В расширение встроено дополнение [nlsclientscript](http://www.yiiframework.com/extension/nlsclientscript/). Включается путем установления соответствующего свойства в TRUE.

        'clientScript' => array(
            'class'=>'ext.SmartClientScript.SmartClientScript',
            'NLSClientScript'=>true,
        ),

## Использование
*   Скопируйте файл `SmartClientScript.php` в директорию `protected` вашего приложения, например `protected/extensions/SmartClientScript/SmartClientScript.php`
*   Подключите компонент в файле конфигурации `protected/config/main.php`
        
        'clientScript' => array(
            'class'=>'ext.SmartClientScript.SmartClientScript',
        ),