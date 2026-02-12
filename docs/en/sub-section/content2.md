# Restricting access to two-step verification setup

## Scenario

> Restricting access to two-step verification setup eliminates the risk of compromised domain user accounts being used to gain access to the security console.

This scenario covers:
*  Preventing users who have not yet configured two-step verification from enabling it without prior approval
*  Managing access to two-step verification setup

Before you proceed, make sure that [two-step verification is enabled for all users](https://support.kaspersky.com/ksc/14.0/211813).


{% cut "Steps" %}

*Чтобы ограничить доступ к настройке двухэтапной проверки*: 

1. В окне свойств Сервера администрирования перейдите в раздел **Authentication security**.

2. Выберите параметр **Require approval to set up two-step verification**.


3. Нажмите кнопку **Edit** ниже параметра, чтобы управлять доступами к настройке двухэтапной проверки:

    * На вкладке **Approved users** добавьте пользователей, которым хотите открыть доступ к настройке.

    * На вкладке **Pending approval** отображаются запросы на доступ к настройке. 
    
    Выберите пользователей и нажмите кнопку **Approve**, чтобы выдать доступ, или **Decline**, чтобы отклонить запрос.

    Подтвердите действие, нажав кнопку **Ok**.

{% endcut %}

As a result, users without two-step verification will not be able to log in. Their attempts to log in will trigger an access request. You will receive notifications on the Monitoring & Reporting Dashboard.

{% note info "" %}

You can see the number of approved users and pending requests in the **General** tab of the Administration Server properties window.

{% endnote %}




