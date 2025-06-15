# deb

Agregar la clave GPG del repositorio  

    curl https://nlbol.github.io/deb/plurios.gpg | gpg --dearmor > /etc/apt/trusted.gpg.d/plurios.gpg

Agregar el repositorio PluriOS  

    echo "deb https://nlbol.github.io/deb/plurios plurios main" | tee /etc/apt/sources.list.d/plurios.list


## Inspiración

La implementación de este repositorio fue un reto inspirado de 'MiniOS Repository'.  
