# Angular 2 QuickStart Source

Este repositorio tiene código TypeScript de [angular.io quickstart](https://angular.io/docs/ts/latest/quickstart.html),
es una base para la mayoría de ejemplos, documentación y pontencialmente un buen punto de partida para tu applicación.

## Crea un nuevo proyecto basado en el QuickStart

Clona este repositorio en un nuevo directorio (e.g., `my-proj`).
```bash
git clone  https://github.com/angular/quickstart  my-proj
cd my-proj
```

Si no tenemos intencion de actualizar el código fuente del repositorio `angular/quickstart`.
Desechamos todo "git-like" borrando el directorio `.git`.
```bash
rm -rf .git
```

### Creamos un nuevo repositorio
Puedes [empezar a escribir código](#comienza-a-desarrollar) ahora ya que hemos terminado y tirado todo por la borda.
Si quisieras preservar todo tu trabajo usando un repositorio, sigue los siguientes pasos.

Inicializa este proyecto como *local git repo* y realiza tu primer commit:
```bash
git init
git add .
git commit -m "Commit Inicial"
```

Crea un repositorio* *remoto para este proyecto en el servicio de tu elección

Obtén la dirección Url (e.g. *`https://github.com/<my-org>/my-proj.git`*) y has push los cambios *locales al repositorio remoto.
```bash
git remote add origin <repo-address>
git push -u origin master
```
### Comienza a desarrollar

Instala npm como lo describe el `package.json` y verifica que funcione:

```bash
npm install
npm start
```
Estas listo para escribir tu aplicación.

Recuerda los scripts npm en `package.json`:

* `npm start` - Corre el compilador y el server al mismo tiempo, los dos en "watch mode".
* `npm run tsc` - Corre TypeScript una sola vez.
* `npm run tsc:w` - Corre el compilador TypeScript en watch mode; el proceso sigue corriendo, esperando por cambios en los archivos TypeScript y re-compila cuando los encuentra.  
* `npm run lite` - Corre el [lite-server](https://www.npmjs.com/package/lite-server), un servidor liviano de archivos estaticos, escrito y mantenido por
[John Papa](https://github.com/johnpapa) y [Christopher Martin](https://github.com/cgmartin)
Con un excelente soporte para aplicaciones Angular que utilizan rutas.
* `npm run typings` - corre la herramienta de typings.
* `npm run postinstall` - llamado por *npm* automatico despues de que complete la intalación de los paquetes con exito. Este script instala las definiciones TypeScript que el app necesita.
