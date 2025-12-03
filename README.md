# deb

Repositorio de paquetes DEB

![PluriOS Banner](plurios.png)

## Instrucciones

Los siguientes comandos se deben ejecutar como **superusuario**:  

**Agregar la clave GPG (curl o wget)**

    curl https://repo.plurios.openit.dev/plurios.gpg | gpg --dearmor > /etc/apt/trusted.gpg.d/plurios.gpg

    wget -q https://repo.plurios.openit.dev/plurios.gpg -O- | gpg --dearmor > /etc/apt/trusted.gpg.d/plurios.gpg


**Agregar el repositorio PluriOS**  

    echo "deb https://repo.plurios.openit.dev/plurios plurios main" | tee /etc/apt/sources.list.d/plurios.list
