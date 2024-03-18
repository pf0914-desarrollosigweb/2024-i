# PF0914 Desarrollo de sistemas de información geográfica en la Web 2024-i

## Contenedor Docker

### Construcción y ejecución
```shell
# Construcción del contenedor Docker
docker build -t pf0914-2024-i .

# Ejecución del contenedor Docker
# (el directorio local debe especificarse en la opción -v)
docker run -d --name pf0914-2024-i \
  -p 8787:8787 \
  -v /home/mfvargas/pf0914-desarrollosigweb/2024-i/github:/home/rstudio \
  -e PASSWORD=pf0914 \
  pf0914-2024-i
```
  
### Acceso
[http://localhost:8787](http://localhost:8787)

### Detención y borrado
```shell
# Detención del contenedor Docker
docker stop pf0914-2024-i

# Borrado del contenedor Docker
docker rm pf0914-2024-i
```