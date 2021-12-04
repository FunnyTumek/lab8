# fibonacci

##Uruchomienie projektu lokalnie
```
npm install - instalacja depencencji dodanych w package.json
npm run build - zbudowanie aplikacji
npm run serve - uruchomienie aplikacji
npm run test:unit - uruchomienie testów aplikacji
```
#Uruchomienie z pomocą docker
```
Sklonowanie repozytorium na dysk poleceniem git clone.
Zbudowanie i uruchomienie kontenera przy pomocy polecenia COMPOSE_DOCKER_CLI_BUILD=1 DOCKER_BUILDKIT=1 docker compose up (wymagana instalacja docker build kit oraz docker compose wersja 2.).
Aplikacja będzie dostępna na http://localhost:8080.
Wyniki testów będą dostępne w konsoli.
```
### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
