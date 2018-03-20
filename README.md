# blowfish

Esta librería es una modificación de sladex-blowfish para ser utilizada correctamente en node.js,
ya que el link disponible en www.npmjs.com hacia el código original en github, lamentablemente, esta roto.

Puedes revisar la versión original del paquete de node en https://www.npmjs.com/package/sladex-blowfish 
y probar sus funciones en http://sladex.org/blowfish.js/


# Forma de uso

- encrypt

	blowfish.encrypt('textoACifrar', 'clave', {cipherMode: 0, outputType: 0});
	
- decrypt

	blowfish.encrypt('textoACifrar', 'clave', {cipherMode: 0, outputType: 0});
	
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