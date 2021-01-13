# Unity-Figma-Gradients
![github-small](cover.jpg)

Библиотека реализующая градиенты Figma в UI в Unity с помощью шейдеров для уменьшения веса билда и отсутствия артефактов сжатия на градиентах.

Для использования необходимо добавить компонент соответствующего типа градиента на RectTransform внутри канваса.

На данный момент есть 4 вида градиентов:

__UIFigmaGradientLinearDrawer__ - линейный градиент

__UIFigmaGradientAngularDrawer__ - конический градиент (не полная поддержка)

__UIFigmaGradientRadialDrawer__ - сферический градиент

__UIFigmaGradinetDiamondDrawer__ - ромбовый градиент 

Для __UIFigmaGradientLinearDrawer__ есть специальная функция для импорта параметров с помощью CSS из Figma. Для этого необходимо скопировать строку из поля _background:_ 
Пример строки: _linear-gradient(0deg, #FECC66 0%, #F83062 100%);_

## Полезные поля классов:
__Gradient Resolution__ - так как градиенты работают через генерацию текстуры размера _1хGradienResolution_ то данное поле позволяет подобрать минимальное подходящее разрешение для вашего градиента.
