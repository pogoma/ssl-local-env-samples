# Przykład dla springboota

## Przyfotowanie keystore'a
```shell script
openssl pkcs12 -export -out store.p12 -inkey private_key.pem -in certificate.pem -certfile ca_certificate.pem 
````
- certificate.pem - certyfikat dla naszej domeny
- private_key.pem - klucz prywatny
- ca_certificate.pem - certyfikat CA (`mkcert -CAROOT`)

## Konfiguracja

```
security.require-ssl=true
server.ssl.key-store=ścieżka/do/store'a/store.p12
server.ssl.keyStoreType=PKCS12
server.ssl.key-store-password=
```


## IntelliJ Run Configuration
Dodajemy nową konfigurację z parametrami
```
security.require-ssl=true
server.ssl.key-store=ścieżka/do/store'a/store.p12
server.ssl.keyStoreType=PKCS12
server.ssl.key-store-password=
```
