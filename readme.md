a. How much data your publisher program will send to the message broker in one
run?

The program publishes 5 messages in one run. Each message contains a UserCreatedEventMessage with user_id and user_name fields. All are sent to the user_created event queue.


b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber
program, what does it mean?

It means both publisher and subscriber connect to the same RabbitMQ broker at localhost on port 5672. This shared connection allows the publisher and subscriber to talk through the same message queue.

