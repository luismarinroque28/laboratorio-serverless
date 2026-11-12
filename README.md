# Laboratorio Serverless con OpenFaaS

## Descripción

En este laboratorio se desarrolló y desplegó una función Serverless utilizando Python y OpenFaaS sobre Kubernetes.

La función muestra un formulario de registro en el navegador. Al completar los datos y enviarlos, genera un archivo JSON que se puede descargar como evidencia.

## Herramientas utilizadas

- Docker Desktop
- Kubernetes
- OpenFaaS
- Python
- Ubuntu WSL2
- Git y GitHub
- Visual Studio Code

## Funcionamiento

1. El usuario accede al formulario desde el navegador.
2. Ingresa su nombre y correo electrónico.
3. La función procesa la información.
4. Se genera un identificador UUID y se registra la fecha y hora.
5. Se crea un archivo JSON con los datos del registro, información del entorno y un hash SHA256.
6. El usuario descarga el archivo generado.

## Archivos principales

- `registro-serverless/`: código fuente de la función.
- `stack.yaml`: configuración del despliegue.
- `install-faas-cli.sh`: script de instalación de faas-cli.
- `registro_*.json`: evidencia de la ejecución.
- `.gitignore`: configuración de archivos excluidos del repositorio.

## Resultado

La función fue desplegada correctamente en OpenFaaS y se comprobó su funcionamiento mediante el formulario web y la descarga del archivo JSON.

## Evidencia

El repositorio incluye un archivo JSON generado durante las pruebas del laboratorio.
