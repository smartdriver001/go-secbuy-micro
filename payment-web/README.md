# Payment web Service

This is the Payment web service

Generated with

```
micro new github.com/wanghaoxi3000/go-secbuy-micro/payment-web --namespace=go.micro.secbuy --alias=payment --type=web
```

## Getting Started

- [Configuration](#configuration)
- [Dependencies](#dependencies)
- [Usage](#usage)

## Configuration

- FQDN: go.micro.secbuy.web.payment
- Type: web
- Alias: payment

## Dependencies

Micro services depend on service discovery. The default is multicast DNS, a zeroconf system.

In the event you need a resilient multi-host setup we recommend consul.

```
# install consul
brew install consul

# run consul
consul agent -dev
```

## Usage

A Makefile is included for convenience

Build the binary

```
make build
```

Run the service
```
./payment-web
```

Build a docker image
```
make docker
```