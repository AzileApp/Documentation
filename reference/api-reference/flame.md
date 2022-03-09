# Flame

{% swagger method="get" path="/api/webhooks/:id/:token" baseUrl="https://flame.azile.app" summary="Displays webhook information" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" type="int" required="true" name="id" %}
Webhook ID
{% endswagger-parameter %}

{% swagger-parameter in="path" required="true" name="token" type="string" %}
Webhook Token
{% endswagger-parameter %}

{% swagger-response status="201: Created" description="Successfully sent webhook request" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="Permission denied" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}

{% swagger-response status="500: Internal Server Error" description="Server Error" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}



{% swagger baseUrl="https://flame.azile.app" method="post" path="/api/webhooks/:id/:token" summary="Sends webhook request." %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" type="int" required="true" name="id" %}
Webhook ID
{% endswagger-parameter %}

{% swagger-parameter in="path" required="true" name="token" type="strig" %}
Webhook Token
{% endswagger-parameter %}

{% swagger-response status="201: Created" description="Successfully sent webhook request" %}
```javascript
{
    "name"="Wilson",
    "owner": {
        "id": "sha7891bikojbkreuy",
        "name": "Samuel Passet",
    "species": "Dog",}
    "breed": "Golden Retriever",
}
```
{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="Permission denied" %}

{% endswagger-response %}

{% swagger-response status="500: Internal Server Error" description="Server Error" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

{% hint style="info" %}

{% endhint %}
