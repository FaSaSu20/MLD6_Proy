# Despliegue de modelos

## Infraestructura

- **Nombre del modelo:**
Modelo para predecir el precio de la energía eléctrica en bolsa.
- **Plataforma de despliegue:**
MLFLOW + RestAPI
- **Requisitos técnicos:**
![image](https://github.com/FaSaSu20/MLD6_Proy/assets/65478386/0d138c0d-c242-4aea-8a9e-ba1c906e1518)
- **Requisitos de seguridad:**
Autenticación de usuarios.
- **Diagrama de arquitectura:**
Interfaz -> Server -> Backend -> Modelo/Predicción

## Código de despliegue

- **Archivo principal:**
4_deployment.ipynb
- **Rutas de acceso a los archivos:**
https://github.com/FaSaSu20/MLD6_Proy/blob/master/scripts/evaluation/4_deployment.ipynb

## Documentación del despliegue

- **Instrucciones de instalación:**
Descargar el modelo: https://drive.google.com/drive/folders/1-zsSGbWRMCUG9PRh98cu1ATmzUyahMTT?usp=drive_link
- **Instrucciones de configuración:**
Cargar el modelo con el metodo de tensorflow  tf.keras.models.load_model()
Instalar las librerais indicadas
- **Instrucciones de uso:**
Los datos deben ser un arreglo de numpy de longitud 4.
- **Instrucciones de mantenimiento:**
Revisar mensualmente si existe drifting en los datos.
