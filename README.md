![image](https://drive.google.com/uc?export=view&id=190XlNLwejgSz5LijH7qJnOK1ORVUfLns)
# Squadcast Event Hooks Middleware

This repository contains the code for the Squadcast Middleware and is intended to be used along with Event Hooks.

## Prerequisites
- git
- NodeJs | npm
- nodemon
### Tip : For Linux Users, just execute the command below to install all the Prerequisites
```
bash dependencies.sh
```

## Getting Started
 - Clone this repo
```sh
git clone https://github.com/highlyUnderrated/Squadcast-EventHooks-Middleware.git
```
- Install dependencies
```sh
npm install
```
- Run
```sh
nodemon start
```
----
## Use Case

### Slack

> URL : https://<Server-IP-Address>:5000/squadcast/middleware/slack

Request Headers :- 
* Slack URL can support multiple channels. To notify channels, just put integers as name of Key value pair & value should be the Slack Webhook. Eg. :
![image](assets/slack.png)

### Trello

> URL : https://<Server-IP-Address>:5000/squadcast/middleware/trello

Request Headers :- 
* To use the Trello webhook, just paste the URL mentioned above in Squadcast Webhook URl box. In the headers, just add "idList", "key" & "token" and their proper values. Eg. : 
![image](assets/trello.png)

* To see your idList, Open a card > Click on Share > Click on Export Json > You'll see a JSON which will contain idList.
* ![image](assets/idList-example.png)
* Tip : To get you own token & key, navigate to : https://trello.com/app-key


### Email

> URL : https://<Server-IP-Address>:5000/squadcast/middleware/email

Request Headers :- 
* To use the email webhook, just paste the URL mentioned above in Squadcast Webhook URl box. In the headers, just add "from_email", "from_password" & "to_email" and their proper values. Eg. : 
![image](assets/email.png)
