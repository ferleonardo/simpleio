# Simple xhr-polling based communication.

- support for router/balancer without sticky sessions (f.e. Heroku)
- optimized for horizontal scaling
- reliable message delivery (built-in delivery confirmation)
- multiplexing on the server and client

# Todo
- tests
- documentation

# Install

    npm i simpleio

    or

    git clone git@github.com:kof/simpleio.git
    make install
    make build


# Run bench

Ensure running mongodb first.

    node bench/adapter

# Api

  - [Client()](#client)
  - [Client.options](#clientoptions)
  - [Client.connect()](#clientconnectdataobject)
  - [Client.disconnect()](#clientdisconnect)
  - [Client.send()](#clientsendmessagemixedcallbackfunction)

## Client()

  Client constructor.

## Client.options

  Defaults.

## Client.connect([data]:Object)

  Start polling.

## Client.disconnect()

  Stop polling.

## Client.send(message:Mixed, [callback]:Function)

  Send message to the server.

