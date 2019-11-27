# blowfish

Esta librería es una modificación de sladex-blowfish para ser utilizada correctamente en node.js,
ya que el link disponible en www.npmjs.com hacia el código original en github, lamentablemente, esta roto.

Puedes revisar la versión original del paquete de node en https://www.npmjs.com/package/sladex-blowfish 
y probar sus funciones en http://sladex.org/blowfish.js/


# Instalación

Ejecuta el siguiente comando desde la consola 
``` 
	npm install sladex-blowfish
``` 

# Configuración en Node

En el directorio 'node_modules' de tu aplicación, buscar la carpeta 'sladex-blowfish' y reemplazar el contenido con los archivos de este proyecto.
Luego, para importar en tu proyecto, usa
``` 
	var blowfish = require("sladex-blowfish");
``` 

# Configuración en Angular

Realiza el import a tu proyecto con
``` 
	import { blowfish } from 'sladex-blowfish';
``` 

# Forma de uso
- Encrypt
``` 
	blowfish.encrypt('textoAEncriptar', 'clave', {cipherMode: 0, outputType: 0});
``` 
	
- Decrypt
``` 
	blowfish.decrypt('textoADesencriptar', 'clave', {cipherMode: 0, outputType: 0});
``` 
	
- cipherMode
``` 
    0 = ECB
    1 = CBC
    2 = PCBC
    3 = CFB
    4 = OFB
    5 = CTR
```

- outputType
```
    0 = Base64
    1 = Hex
    2 = String
    3 = Raw
```
