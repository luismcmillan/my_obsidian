[[Docker]]
[[Shell]]
```Shell
# Installation und Setup
docker --version  # Zeigt die aktuell installierte Docker-Version an.

# Grundlegende Befehle
docker images  # Listet alle lokal gespeicherten Docker-Images auf.
docker ps  # Zeigt alle laufenden Container an.
docker ps -a  # Zeigt alle Container an, auch die gestoppten.

docker start <container_id>  # Startet einen gestoppten Container.
docker stop <container_id>  # Stoppt einen laufenden Container.
docker rm <container_id>  # Löscht einen gestoppten Container.
docker rmi <image_id>  # Löscht ein Docker-Image von der Festplatte.

# Container erstellen und verwalten
docker run <image_name>  # Startet einen neuen Container aus dem angegebenen Image.
docker run -d <image_name>  # Startet den Container im Hintergrund (detached mode).
docker attach a043d
docker run -it <image_name> /bin/bash  # Startet einen Container und öffnet eine interaktive Shell.

docker logs <container_id>  # Zeigt die Logs eines Containers an.
docker exec -it <container_id> /bin/bash  # Öffnet eine Shell in einem laufenden Container.

# Docker Volumes und Netzwerke
docker volume create <volume_name>  # Erstellt ein neues Docker-Volume.
docker volume ls  # Listet alle Docker-Volumes auf.

docker network create <network_name>  # Erstellt ein neues Docker-Netzwerk.
docker network ls  # Listet alle Docker-Netzwerke auf.
docker network connect <network_name> <container_id>  # Verbindet einen Container mit einem Docker-Netzwerk.

# Docker Compose
docker-compose up  # Startet die in der docker-compose.yml definierte Anwendung.
docker-compose up -d  # Startet die Anwendung im Hintergrund.
docker-compose down  # Stoppt und entfernt alle Container, Netzwerke und Volumes, die durch docker-compose up erstellt wurden.

# Docker Images erstellen
docker build -t <image_name> .  # Erstellt ein Docker-Image aus einem Dockerfile im aktuellen Verzeichnis.

# Docker Registries
docker push <registry_url>/<username>/<image_name>:<tag>  # Pusht ein Docker-Image zu einer Docker-Registry.
docker pull <registry_url>/<username>/<image_name>:<tag>  # Lädt ein Docker-Image von einer Docker-Registry herunter.

# Sonstiges
docker system prune  # Entfernt ungenutzte Docker-Daten (Images, Container, Volumes, Netzwerke).
docker run --rm <image_name>  # Startet einen Container und entfernt ihn nach Beendigung automatisch.

```