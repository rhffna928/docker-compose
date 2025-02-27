services:
  rabbitmq-1:
    image: rabbitmq:4.0.7-management
    container_name: rabbitmq-1
    hostname: rabbitmq-1
    ports:
      - 15672:15672
      - 5672:5672
    environment:
      RABBITMQ_ERLANG_COOKIE: rabbitmqCookie
      RABBITMQ_DEFAULT_USER: admin
      RABBITMQ_DEFAULT_PASS: 1234

  rabbitmq-2:
    image: rabbitmq:4.0.7-management
    container_name: rabbitmq-2
    hostname: rabbitmq-2
    environment:
      RABBITMQ_ERLANG_COOKIE: rabbitmqCookie
      RABBITMQ_DEFAULT_USER: admin
      RABBITMQ_DEFAULT_PASS: 1234
    depends_on:
      - rabbitmq-1

  rabbitmq-3:
    image: rabbitmq:4.0.7-management
    container_name: rabbitmq-3
    hostname: rabbitmq-3
    environment:
      RABBITMQ_ERLANG_COOKIE: rabbitmqCookie
      RABBITMQ_DEFAULT_USER: admin
      RABBITMQ_DEFAULT_PASS: 1234
    depends_on:
      - rabbitmq-1
