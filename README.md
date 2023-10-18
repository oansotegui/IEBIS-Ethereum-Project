# IEBIS Ethereum Project

Este proyecto se compone de un contrato Ethereum y una DApp asociada.

## Estructura del Proyecto

- `/contract`: Contiene un proyecto Truffle con el código fuente del Smart Contract y los Test.
- `/dapp`: Contiene el código fuente de la DApp.

## Clonación del Proyecto

Para clonar este proyecto y sus submódulos, ejecuta:

```bash
git clone --recurse-submodules https://github.com/oansotegui/IEBIS-Ethereum-Project.git
```

## Trabajando con Submódulos

Los submódulos permiten trabajar con repositorios dentro de otros repositorios. Aquí hay algunos comandos útiles para trabajar con submódulos:

Obtener las Últimas Actualizaciones de los Submódulos:

```bash
git submodule update --remote
```

## Cambiar a una Rama Específica en un Submódulo:

Dentro del directorio de un submódulo, puedes cambiar a otra rama y trabajar en ella como lo harías en cualquier otro repositorio de git.

```bash
cd contract
git checkout <branch-name>
```

## Hacer Commit de Cambios en los Submódulos:

Si realizas cambios dentro de un submódulo, estos se reflejarán en el repositorio principal como un cambio en el commit al que apunta el submódulo. Para actualizar el repositorio principal con estos cambios, necesitas hacer commit de los submódulos en el repositorio principal.

```bash
git add contract
git commit -m "Updated the contract submodule."
git push
```

## Clonar el Repositorio Principal con Submódulos:

Cuando clones el repositorio principal, los submódulos estarán vacíos. Para clonar el repositorio principal y todos los submódulos en un solo comando, usa:

```bash
git clone --recurse-submodules https://github.com/oansotegui/IEBIS-Ethereum-Project.git
```

Si ya has clonado el repositorio principal y deseas clonar los submódulos, usa:

```bash
git submodule update --init
```

