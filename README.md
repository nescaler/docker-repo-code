# Clone the repository
git clone https://github.com/nescaler/docker-repo-code.git

# docker-repo-code
Repository used to print info required for docker task

# Creamos una imagen que se llamara myjavaapi usando el -t, que se encargara de tagearla , ponemos punto para el contexto
docker build -t myjavaapi .

# Creamos el contenedor con el nombre myjavaapp que tendra expuesto el puerto del home como 9009 y el containedor tiene el expuesto el puerto 8080, usando la imagen myjavaapi:latest
docker run -d --name myjavaapp -p 9009:8080 myjavaapi:latest

# Use API application url
http://10.24.48.239:9009/system-data/
