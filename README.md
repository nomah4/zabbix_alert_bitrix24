# zabbix_alert_bitrix24
Script bash to integrate zabbix alert messages to Bitrix24 channel

First you have to make a webhook in Bitrix24 by going into "Developer resources" -> "Other" -> "Incoming webhooks".
Then choose form methodes "im.message.add" and save.
Copy the URL to script in parameter "webhook_url"
Make a new chat that will be called for ex. "Zabbix"

Use jq to make valid message to JSON


In Zabbix 

Alerts - Media types - Create media type

Select Script
Script parameters - 
1. enter you ChatID
2. {ALERT.MESSAGE}

Also you can config Message Template
