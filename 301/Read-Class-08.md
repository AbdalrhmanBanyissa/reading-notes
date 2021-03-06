# APIs

## API Design Best Practices

A well designed API should aim to support:

- Platform independence

  - Any client should be able to call the API regardless of how the API is implemented internally. This requires using standard protocols, and having a mechanism whereby the client and the web service can agree on the format of the data to exchange

- Service evolution

  - The web API should be able to evolve and add functionality independently from client applications. As the API evolves, existing client applications should continue to function without modification. All functionality should be discoverable so that client applications can fully use it.

REST = Representational State Transfer - an architectural approach to designing web services, a style for building distributed systems based on hypermedia.

Many web APIs use JSON as the exchange format.

## Documentation for SuperAgent

SuperAgent is a light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js.
