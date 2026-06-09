# ZenRay public shard

Dépôt **public** d'assets ZenRay.

Les fichiers sont nommés par leur **empreinte SHA-256** (`ab/cd/<hash>.<ext>`) accompagnés
d'une vignette `.webp`, et servis via **jsDelivr** (cache immuable pinné sur le commit).
Aucun nom humain n'apparaît : seuls des chemins hashés.

Quand un shard approche ~5 Go, l'application en crée automatiquement un suivant. L'état de
remplissage est suivi dans un fichier d'état du dépôt privé `zenray-data`.

Ne rien committer à la main ici : toutes les écritures passent par l'API serveur (Git Data API).
