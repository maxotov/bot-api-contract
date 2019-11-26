---
title: FormClosed
sidebar: home_sidebar
keywords: update, form, form closed
permalink: formclosed.html
toc: true
folder: Types
---

## Desciprtion

<p> This object represents update  about form being closed by a user.
</p>

## Structure

| Variable  | Obligative  |Type| Description
|---|:---:|---|---|
| updateId  | true |String| Backend ID of the update |
| formId  | true |String| Backend ID of a form |
| dialog  | true |Peer |  Dialog in which form was closed |
| sender  | true |Peer |  User who closed a form  |
| type  | true | String | "FormClosed" value must be filled

## Sample object

```
               {
                 "updateId" : "e7377c24-d975-4e5b-b4f7-b1aeaa12b243",
                 "type" : "FormClosed",
                 "formId" : "80f3d865-0210-4604-8c57-b959b9423a00",
                 "dialog" : {
                   "type" : "GROUP",
                   "id" : "e3158a4a-1f92-41d2-b991-7ee95bed3918",
                   "name" : "Aitu"
                 },
                 "sender" : {
                   "type" : "USER",
                   "id" : "3a17518d-63d4-4d63-9c46-9c312588779a",
                   "username" : "TestUserName",
                   "lastName" : "TestlastName",
                   "firstName" : "testfirstName"
                 }
               }
```