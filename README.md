## a. What is AMQP?

**AMQP** stands for **Advanced Message Queuing Protocol**.  
It is an open standard protocol for message-oriented middleware. AMQP enables systems to communicate by sending messages between clients and servers, often used to connect microservices or distributed systems. It is widely used for reliable messaging, queuing, publish/subscribe, and routing, and is implemented by message brokers like **RabbitMQ**.

---

## b. What does `guest:guest@localhost:5672` mean?

This is a **connection string** for an AMQP broker (like RabbitMQ).

### `guest:guest`
- The **first `guest`** is the **username**.
- The **second `guest`** is the **password**.

### `localhost:5672`
- **`localhost`** is the **hostname** of the server running the AMQP broker. `localhost` means the broker is running on the same computer as the client.
- **`5672`** is the **port number** that AMQP brokers (like RabbitMQ) listen on for client connections.

---

### **Full meaning**

- Connect to the AMQP server running on local computer (`localhost`)
- Use port `5672` (default for AMQP)
- Log in with username `guest` and password `guest`