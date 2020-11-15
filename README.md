# Notebook

Personal Notebook

## Step per mettere su l'ambiente

Possiamo utilizzare le immagini Docker presenti [qui](https://hub.docker.com/r/klakegg/hugo/).
Personalmente utilizzo il tag `klakegg/hugo:0.78.0-ext-alpine`.

Per lo sviluppo è ideale mappare la directory di lavoro presente sulla macchian host come volume del
container Docker.

Per iniziare da zero è necessario lanciare la shell sul container, per invocare i comandi hugo per la
creazione del sito. il comando da eseguire è ad esempio

```shell
docker run --rm -it --name hugo-book-container -v <LOCAL-DEV-PATH>:/src klakegg/hugo:0.78.0-ext-alpine shell
```

Adesso per creare nuovo sito entriamo con la shell e con i seguenti comandi (utilizziamo ad esempio
[questo tema](https://github.com/alex-shpak/hugo-book) che ho in fork):

```shell
hugo new site hugo-book-site
cd hugo-book-site
git init
git submodule add https://github.com/j4bberwocky/hugo-book.git themes/book
echo 'theme = "book"' >> config.toml
cp -R themes/book/exampleSite/content .
```

Adesso il sito è pronto per essere servito. Sarà necessario creare un binding tra la porta su
cui Hugo è in ascolto nel container e una porta della macchina locale. Si lancia di nuovo la shell

```shell
docker run --rm --name hugo-book-container -it -p 1313:1313 -v <LOCAL-DEV-PATH>:/src klakegg/hugo:0.78.0-ext-alpine shell
```

Infine serviamo il sito

```shell
hugo serve
```
