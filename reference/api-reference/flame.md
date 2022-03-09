# Flame



{% swagger baseUrl="https://flame.azile.app" method="post" path="/api/webhooks/:id/:token" summary="Sends webhook request." %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" %}

{% endswagger-parameter %}

{% swagger-parameter in="path" type="int" required="true" name="id" %}
Webhook ID
{% endswagger-parameter %}

{% swagger-parameter in="path" required="true" name="token" type="strig" %}
Webhook Token
{% endswagger-parameter %}

{% swagger-response status="200" description="Successfully sent we" %}
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

{% swagger-response status="401" description="Permission denied" %}

{% endswagger-response %}
{% endswagger %}

## Updating a pet

{% hint style="info" %}
**Good to know:** This API method was auto-generated from an example Swagger file. You'll see that it's not editable – that's because the contents are synced to an URL! Any time the linked file changes, the documentation will change too.
{% endhint %}
