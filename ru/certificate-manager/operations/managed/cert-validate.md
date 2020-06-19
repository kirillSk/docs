# Прохождение процедуры проверки прав на домены

Чтобы пройти процедуру проверки прав на домены:

{% list tabs %}

- Консоль управления

    1. В [консоли управления]({{ link-console-main }}) выберите каталог, в котором будет создан сертификат.
    1. В списке сервисов выберите **{{ certificate-manager-name }}**.
    1. Выберите в списке сертификат, для которого небходимо пройти процедуру проверки и нажмите на него.
    1. В открывшемся окне в блоке **Проверка прав на домены** будет указана информация для прохождения процедуры проверки прав. Подробнее читайте в разделе [{#T}](../../concepts/challenges.md).
    1. После успешного прохождения проверки прав на домен, статус проверки домена в блоке **Проверка прав на домены** изменится на `Valid`.
    1. После того, как статус проверки прав всех доменов изменится на `Valid`, сертификат будет выпущен и перейдет в статус `Issued`. 

{% endlist %}