![image](assets/SQ.svg)
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

> URL : https://Server-IP-Address:5000/squadcast/middleware/slack

Request Headers :- 
* Slack URL can support multiple channels. To notify channels, just put integers as name of Key value pair & value should be the Slack Webhook. Eg. :
![image](assets/slack.png)

### Trello

> URL : https://Server-IP-Address:5000/squadcast/middleware/trello

Request Headers :- 
* To use the Trello webhook, just paste the URL mentioned above in Squadcast Webhook URl box. In the headers, just add "idList", "key" & "token" and their proper values. Eg. : 
![image](assets/trello.png)

* To see your idList, Open a card > Click on Share > Click on Export Json > You'll see a JSON which will contain idList.
* ![image](assets/idList-example.png)
* Tip : To get you own token & key, navigate to : https://trello.com/app-key


### Email

> URL : https://Server-IP-Address:5000/squadcast/middleware/email

Request Headers :- 
* To use the email webhook, just paste the URL mentioned above in Squadcast Webhook URl box. In the headers, just add "from_email", "from_password", "to_email" & "SMTP" and their proper values. Eg. : 
![image](assets/email.png)

List of SMTP Providers Supported : -
* Service names are case insensitive : 
"126"
"163"
"1und1"
"AOL"
"DebugMail"
"DynectEmail"
"FastMail"
"GandiMail"
"Gmail"
"Godaddy"
"GodaddyAsia"
"GodaddyEurope"
"hot.ee"
"Hotmail"
"iCloud"
"mail.ee"
"Mail.ru"
"Maildev"
"Mailgun"
"Mailjet"
"Mailosaur"
"Mandrill"
"Naver"
"OpenMailBox"
"Outlook365"
"Postmark"
"QQ"
"QQex"
"SendCloud"
"SendGrid"
"SendinBlue"
"SendPulse"
"SES"
"SES-US-EAST-1"
"SES-US-WEST-2"
"SES-EU-WEST-1"
"Sparkpost"
"Yahoo"
"Yandex"
"Zoho"
"qiye.aliyun"


### Telegram

> URL : https://Server-IP-Address:5000/squadcast/middleware/telegram

Steps :-
1. `Important` : Before starting, create your own Telegram Bot : https://core.telegram.org/bots#6-botfather
2. Paste the Telegram Bot Token in the `telegram_bot_token` in .env file. Also change the `telegram_bot_start` variable's value to "yes". Eg. : 
![image](assets/telegram_env.png)
3. Now you can start the server, Refer Getting Started - Step 3.
4. To use the telegram webhook, just paste the URL mentioned above in Squadcast Webhook URl box. In the headers, just add "chatId" and its proper value. Eg. : 
![image](assets/telegram.png)
* Tip : To get you own chatId, follow this article : https://www.alphr.com/find-chat-id-telegram/