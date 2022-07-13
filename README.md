**For balena's current cloud integration tools, see the [Provision with cloud IoT](https://www.balena.io/docs/learn/develop/cloud-iot-provisioning/aws/) docs, [aws-iot-provision](https://github.com/balena-io-examples/aws-iot-provision) repo, and [cloud-relay](https://github.com/balena-io-examples/cloud-relay) repo.**

## Balena AWS IoT Example Project

This is a sample project on how to connect a balena device to a AWS IoT MQTT Broker. 
The `main.py` program subscribes to a topic called `balena/payload_test` while publishing to `balena/payload_write_test` with an incremental number every 5 seconds.

### Environment Varibles:

| Name             | Value                                     | Defaut                           |
|------------------|-------------------------------------------|----------------------------------|
| AWS_ENDPOINT     | application endpoint                      | data.iot.us-east-1.amazonaws.com |
| AWS_PRIVATE_CERT | thing private key encoded in base64       |                                  |
| AWS_ROOT_CERT    | aws root certificate encoded in base64    |                                  |
| AWS_THING_CERT   | thing certificate                         |                                  |
| AWS_PORT         | change in case you setup a different port | 8883                             |
