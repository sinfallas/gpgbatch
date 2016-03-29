# gpgbatch

[![GitHub license](https://sinfallas.files.wordpress.com/2016/02/gpl.png)](https://github.com/sinfallas/gpgbatch/blob/master/LICENSE)
[![DOI](https://zenodo.org/badge/4102/sinfallas/gpgbatch.svg)](https://zenodo.org/badge/latestdoi/4102/sinfallas/gpgbatch)
[![Build Status](https://travis-ci.org/sinfallas/gpgbatch.svg?branch=master)](https://travis-ci.org/sinfallas/gpgbatch)

Crea llaves GPG mediante un proceso por lotes; para introducir la informacion necesaria para crear las llaves se debe crear un archivo llamado "datos.txt" con la siguiente información:

```bash
longitud:nombre:apellido:su@email.com:vencimiento:clave
```

Ejemplo:

```bash
2048:jose:perez:casa@casa.com:2y:miclave1234
```

Si desea que las llaves publicas se envien a los keyserver debe ejecutar el script de la siguiente forma:

```bash
./gpgbatch enviar
```
