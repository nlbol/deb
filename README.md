# deb

Repositorio de paquetes DEB - PluriOS

![PluriOS Banner](plurios.png)

## Instrucciones

Los siguientes comandos se deben ejecutar como **superusuario**:  

**Agregar la clave GPG del repositorio (curl o wget)**

    curl https://nlbol.github.io/deb/plurios.gpg | gpg --dearmor > /etc/apt/trusted.gpg.d/plurios.gpg

    wget -q https://nlbol.github.io/deb/plurios.gpg -O- | gpg --dearmor > /etc/apt/trusted.gpg.d/plurios.gpg


**Agregar el repositorio PluriOS**  

    echo "deb https://nlbol.github.io/deb/plurios plurios main" | tee /etc/apt/sources.list.d/plurios.list

