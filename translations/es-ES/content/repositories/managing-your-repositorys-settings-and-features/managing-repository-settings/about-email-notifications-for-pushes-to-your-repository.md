---
title: Acerca de las notificaciones por correo electrónico para las inserciones en tu repositorio
intro: Puedes elegir enviar notificaciones por correo electrónico automáticamente a una dirección en específico cuando alguien suba información a tu repositorio.
permissions: People with admin permissions in a repository can enable email notifications for pushes to your repository.
redirect_from:
  - /articles/managing-notifications-for-pushes-to-a-repository/
  - /articles/receiving-email-notifications-for-pushes-to-a-repository/
  - /articles/about-email-notifications-for-pushes-to-your-repository/
  - /github/receiving-notifications-about-activity-on-github/about-email-notifications-for-pushes-to-your-repository
  - /github/administering-a-repository/about-email-notifications-for-pushes-to-your-repository
  - /github/administering-a-repository/managing-repository-settings/about-email-notifications-for-pushes-to-your-repository
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Repositories
shortTitle: Enviar notificaciones por correo electrónico para las subidas
---

{% data reusables.notifications.outbound_email_tip %}

Cada notificación por correo electrónico para una subida a un repositorio enumera las confirmaciones nuevas y las vincula a una diferencia que solo contenga esas confirmaciones. En la notificación por correo electrónico verás:

- El nombre del repositorio donde se realizó la confirmación.
- La rama en la que se realizó la confirmación.
- El SHA1 de la confirmación, incluido un enlace a la diferencia en {% data variables.product.product_name %}.
- El autor de la confirmación.
- La fecha en que se realizó la confirmación.
- Los archivos que fueron modificados como parte de la confirmación.
- El mensaje de confirmación

Puedes filtrar las notificaciones por correo electrónico que recibes para las inserciones en un repositorio. Para obtener más información, consulta la sección {% ifversion fpt or ghae or ghes or ghec %}"[Configurar notificaciones](/github/managing-subscriptions-and-notifications-on-github/configuring-notifications#filtering-email-notifications){% else %}"[Acerca de los mensajes de notificación por correo electrónico](/github/receiving-notifications-about-activity-on-github/about-email-notifications)". También puedes apagar las notificaciones por correo electrónico para las cargas de información. Para obtener más información, consulta la sección "[Escoger el método de entrega para las notificaciones](/enterprise/{{ currentVersion }}/user/github/receiving-notifications-about-activity-on-github/choosing-the-delivery-method-for-your-notifications){% endif %}".

## Habilitar las notificaciones por correo electrónico para las subidas de información en tu repositorio

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-settings %}
{% data reusables.repositories.sidebar-notifications %}
5. Escribe hasta dos direcciones de correo electrónico, separadas por espacio en blanco, donde quieras que se envíen las notificaciones. Si quieres enviar los correos electrónicos a más de dos cuentas, configura una de las direcciones de correo electrónico a una dirección de correo electrónico del grupo. ![Cuadro de texto dirección de correo electrónico](/assets/images/help/settings/email_services_addresses.png)
1. Si operas tu propio servidor, puedes verificar la integridad de los correos electrónicos a través del **Encabezado aprobado**. El **Encabezado aprobado** es un token o un secreto que tecleas en este campo y que se envía con el correo electrónico. Si el encabezado que está como `Approved` en un correo electrónico empata con el token, puedes confiar en que dicho correo es de {% data variables.product.product_name %}. ![Caja de texto de correo de encabezado aprobado](/assets/images/help/settings/email_services_approved_header.png)
7. Da clic en **Configurar notificaciones**. ![Botón de configurar notificaciones](/assets/images/help/settings/setup_notifications_settings.png)

## Leer más
{% ifversion fpt or ghae or ghes or ghec %}
- "[Acerca de las notificaciones](/github/managing-subscriptions-and-notifications-on-github/about-notifications)"
{% else %}
- "[Acerca de las notificaciones](/enterprise/{{ currentVersion }}/user/github/receiving-notifications-about-activity-on-github/about-notifications)"
- "[Escoger el método de entrega para tus notificaciones](/enterprise/{{ currentVersion }}/user/github/receiving-notifications-about-activity-on-github/choosing-the-delivery-method-for-your-notifications)"
- "[Acerca de las notificaciones por correo electrónico](/enterprise/{{ currentVersion }}/user/github/receiving-notifications-about-activity-on-github/about-email-notifications)"
- "[Acerca de las notificaciones web](/enterprise/{{ currentVersion }}/user/github/receiving-notifications-about-activity-on-github/about-web-notifications)"{% endif %}
