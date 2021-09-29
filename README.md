## Wygenerowanie i instalacja lokalnego CA
```shell script
mkcert -install
```
* Do instalacji wymagane jest sudo

## Sprawdzenie gdzie leży wygenerowany cert CA
```shell script
mkcert -CAROOT
```

## Wygenerowanie certyfikatu dla domeny
```shell script
mkcert localhost
```

## Przykłady implementacji
- [Spring Boot](springboot/README.md)
- [Angular+nx](angular/README.md)
