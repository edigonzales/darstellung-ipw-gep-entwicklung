# darstellung-ipw-gep-entwicklung

## QGIS 2.18
Für Erstellung der QML für AGI SO.

```
cd vagrant/qgis218
vagrant up
ssh -X -p 2020 vagrant@127.0.0.1 qgis
```

oder mit _x2go_ (xfc4). 

- Passwort `vagrant`.
- Host-IP (für DB-Connection): `192.168.56.1`


## QGIS 3.16
Für das Editieren von Daten.

```
cd vagrant/qgis218
vagrant up
ssh -X -p 2021 vagrant@127.0.0.1 qgis
```

oder mit _x2go_ (xfc4). 

- Passwort `vagrant`.
- Host-IP (für DB-Connection): `192.168.56.1`

## Datenbank und Geoserver

```
docker-compose up
```

### Datenbank

Die Daten bleiben auch z.B. nach `docker-compose stop` oder `docker-compose down` erhalten. Falls man mit leeren DBs neu starten möchte:

```
docker-compose down
docker volume prune
```

Credentials: 

* Hostname: `localhost`
* Port: `54321`
* DB-Name: `edit`
* Benutzer: `gretl` (für Lese- und Schreibzugriff) oder `admin` (zum Anlegen von Schemen, Tabellen usw.); das Passwort lautet jeweils gleich wie der Benutzername


### Geoserver

Credentials: `admin / geoserver`

## VSA-DSS-mini Datenmodell 

### Leere Tabellen und Schema anlegen (lokal)

```

```
