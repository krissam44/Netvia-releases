# Netvia

Analyseur de réseau local pour Windows et Linux : trouvez tous les appareils de votre réseau, identifiez-les et ouvrez leurs services en un clic.

## Fonctionnalités

- **Découverte des appareils** par ping, ARP, DNS, mDNS et NetBIOS
- **Identification du type** (box, ordinateur, téléphone, NAS, objet connecté, ESP32, Shelly…), avec la possibilité de **créer vos propres types** et de reclasser chaque appareil
- **Analyse des ports** courants, ou des 65 535 ports d'un appareil
- **Ouverture des services** trouvés : navigateur, PuTTY / SSH, bureau à distance
- **Noms personnalisés**, repérage des **nouveaux appareils**
- **Import et export CSV**
- Thème sombre ou clair

## Téléchargement

Rendez-vous dans les [**Releases**](../../releases/latest) et choisissez le fichier adapté :

| Système | Fichier |
|---|---|
| Windows 10 / 11 (64 bits) | `Netvia-Setup-x.y.z.exe` |
| Debian 12+, Ubuntu 22.04+, Linux Mint 21+ | `netvia_x.y.z_amd64.deb` |

## Installation

### Windows

Lancez `Netvia-Setup-x.y.z.exe`. L'installation ne demande pas de droits administrateur et ajoute Netvia au menu Démarrer.

> L'installateur n'est pas signé numériquement : Windows SmartScreen peut afficher « Windows a protégé votre ordinateur ». Cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**.

Pour désinstaller : **Paramètres › Applications**.

### Debian / Ubuntu / Mint

```bash
sudo apt install ./netvia_x.y.z_amd64.deb
```

Pour désinstaller : `sudo apt remove netvia`.

## Réglages

Les réglages (noms des appareils, types personnalisés, thème…) sont enregistrés dans :

| Système | Fichier |
|---|---|
| Windows | `%APPDATA%\Netvia\settings.txt` |
| Linux   | `~/.config/Netvia/settings.txt` |
