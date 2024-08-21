# Avail Node Template
This is a template to start a JSON-RPC node on the Avail Network. 

## Personalization
You can change the node name at line 21 in deploy.yaml. This name will be used to identify your node on the [Telemetry Dashboard](https://telemetry.avail.so/#list/0xb91746b45e0346cc2f815a520b9c6cb4d5c0902af848db0a80f85932d2e8276a).

## Testing

To check the node status, you can run the following command:
```bash
curl --location "http://[providerHostname]:[forwarded port of 9944]/"     --header 'Content-Type: application/json'     --data '{"id":"1", "jsonrpc":"2.0", "method": "system_health"}'
```

Make sure to replace `[providerHostname]` with the hostname of the provider and `[forwarded port of 9944]` with the port which is forwarded to the provider's 9944 port.