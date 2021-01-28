# Design Plone Buildout #

Buildout base per un'installazione di Agid2 + Volto.

## Installazione ##

Ci sono 3 possibili profili (nella cartella `profiles`):

- development
- staging
- production

Per prima cosa, bisogna creare un virtualenv per Python 3 nel modo in cui si preferisce (virtualenv, pipenv, pyenv).

Una volta attivato, basta scegliere il profilo da usare (per esempio development.cfg) ed eseguire i seguenti comandi:

```bash
pip install -r requirements.txt
ln -s profiles/development.cfg buildout.cfg
buildout -N
```
