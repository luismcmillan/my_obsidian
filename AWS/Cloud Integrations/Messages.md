[[SQS - Simple Queue Service]]: 
- Queue service in AWS
- Multiple Producers, messages are kept up to 14 days
- Multiple Consumers share the read and delete messages when done
- Used to **decouple** applications in AWS
[[Amazon SNS - Simple Notification Service]]:
- Notification service in AWS
- Subscribers:Email, Lambda, SQS, HTTP, Mobile...
- Multiple Subscribers, send all messages to all of them
- No message retention
[[Amazon Kinesis]]: real-time data streaming, persistence and analysis
[[Amazon MQ]]: managed message broker for ActiveMQ and RabbitMQ in the cloud (MQTT,AMQP.. protocols)