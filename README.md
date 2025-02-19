# Crearem diferents bases de dades en MongoDB

## Nivell 1: Òptica

Una òptica, anomenada “Cul d'Ampolla”, vol informatitzar la gestió dels clients/es i vendes d'ulleres.

### Requisits de l'òptica

1. **Proveïdors**:
   - Nom
   - Adreça (carrer, número, pis, porta, ciutat, codi postal, país)
   - Telèfon
   - Fax
   - NIF

2. **Ulleres**:
   - Marca
   - Graduació de cada vidre
   - Tipus de muntura (flotant, pasta o metàl·lica)
   - Color de la muntura
   - Color de cada vidre
   - Preu

3. **Clients/es**:
   - Nom
   - Adreça postal
   - Telèfon
   - Correu electrònic
   - Data de registre
   - Client/a que li ha recomanat (opcional)

4. **Vendes**:
   - Empleat/da que ha realitzat la venda
   - Data/hora de la venda

### Exercici 1
Imagina que tenim la següent interfície gràfica, des del punt de vista d’un client de l'Òptica. Com dissenyaries la base de dades que facilités la informació?
![Client view](.Imagen1PHP.jpg)
### Exercici 2
I si el punt de vista fos de la interfície fossin les ulleres?
![Glass view](.Imagen2PHP.jpg)

---

## Nivell 2: Comandes de menjar a domicili

T’han contractat per a dissenyar una web que permeti fer comandes de menjar a domicili per Internet.
Aquesta és la vista que hem de fer possible: 
![Order view](.Imagen3PHP.jpg)

### Requisits del sistema

1. **Clients/es**:
   - Identificador únic
   - Nom
   - Cognoms
   - Adreça
   - Codi postal
   - Localitat
   - Província
   - Número de telèfon

2. **Comandes**:
   - Identificador únic
   - Data/hora de realització
   - Tipus de comanda (domicili o recollida en botiga)
   - Quantitat de productes seleccionats
   - Preu total
   - Nota amb informació addicional

3. **Productes**:
   - Identificador únic
   - Nom
   - Descripció
   - Imatge
   - Preu
   - Categories (per a pizzes)

4. **Botigues**:
   - Identificador únic
   - Adreça
   - Codi postal
   - Localitat
   - Província

5. **Empleats/des**:
   - Identificador únic
   - Nom
   - Cognoms
   - NIF
   - Telèfon
   - Rol (cuiner/a o repartidor/a)

6. **Repartiments**:
   - Repartidor/a
   - Data/hora del lliurament

---

## Nivell 3: YouTube

Tractarem de fer un model senzill de com seria la base de dades per a una versió reduïda de YouTube.
Aquesta és la vista que hem de fer possible: 
![Video view](.Imagen4PHP.jpg)
### Requisits del sistema

1. **Usuaris/es**:
   - Identificador únic
   - Email
   - Password
   - Nom d'usuari/ària
   - Data de naixement
   - Sexe
   - País
   - Codi postal

2. **Vídeos**:
   - Identificador únic
   - Títol
   - Descripció
   - Grandària
   - Nom de l'arxiu de vídeo
   - Durada del vídeo
   - Thumbnail
   - Nombre de reproduccions
   - Nombre de likes
   - Nombre de dislikes
   - Estat (públic, ocult, privat)
   - Etiquetes
   - Usuari/ària que publica el vídeo
   - Data/hora de publicació

3. **Canals**:
   - Identificador únic
   - Nom
   - Descripció
   - Data de creació

4. **Subscripcions**:
   - Usuari/ària que es subscriu
   - Canal al qual es subscriu

5. **Likes/Dislikes**:
   - Usuari/ària que dóna like/dislike
   - Vídeo al qual es dóna like/dislike
   - Data/hora de l'acció

6. **Playlists**:
   - Identificador únic
   - Nom
   - Data de creació
   - Estat (pública o privada)

7. **Comentaris**:
   - Identificador únic
   - Text del comentari
   - Data/hora del comentari
