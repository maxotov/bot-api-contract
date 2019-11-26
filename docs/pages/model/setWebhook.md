---
title: setWebhook
sidebar: home_sidebar
keywords: Webhook,setting webhook, updates
permalink: setwebhook.html
toc: true
folder: Types
---

![Types](images/SetWebhook.png "setWebhook")

## Desciprtion

<p> This method is for setting an url for backend to send updates for service. 
</p>
<p> On succes empty response with http code 200 is returned.
</p>

## Endpoint

/https://messapi.btsdapps.net/bot/v1/webhook/

## Structure

| Variable  | Obligative  | Type| Validation| Description
|---|:---:|---|---|---|
| url | true | String | Size of url should be <= 200 |URL set to get updates on |

## URL validation

URL should comply with URL living standart (https://url.spec.whatwg.org).
HTTPS protocol should be defined for this url.

## Sample object

```
{
  "url" : "https://user:pass@www.example.com:81/path/index.php?query=toto+le+heros#top"
}
```