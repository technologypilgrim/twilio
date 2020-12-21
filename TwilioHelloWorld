from twilio.rest import Client 
import os
 
accountSid = os.environ['TWILIO_SID']
authToken = os.environ['TWILIO_AUTH_TOKEN']
toPhone = os.environ['TWILIO_TO_PHONE']
messagingServiceId = os.environ['TWILIO_MSG_SVC']
msgBody = 'Hello World By Techpilgrim'

client = Client(accountSid, authToken)
message = client.messages.create(to=toPhone, messaging_service_sid=messagingServiceId, body=msgBody)
print('SMS Sent: Message Id: ' + message.sid)
