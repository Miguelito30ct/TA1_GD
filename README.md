# Indicadores de Calidad de Datos

Este proyecto tiene como objetivo obtener datos de tres fuentes públicas: noticias, temperatura y tipo de cambio, y analizar la calidad de los datos obtenidos. Los datos se extraen a través de APIs públicas, y se validan en base a indicadores de calidad como la **completitud**, **exactitud**, **consistencia** y **actualización**.

## Indicadores de Calidad

### Completitud
Se asegura que los datos de noticias no tengan valores nulos en los campos importantes como el título y la descripción. Si alguno de estos valores falta, la noticia es descartada.

### Exactitud
Verificamos que la temperatura y el tipo de cambio obtenidos estén dentro de rangos lógicos y esperados, para evitar datos erróneos.

### Consistencia
Comprobamos que los datos extraídos de las diferentes fuentes sean coherentes entre sí y con las expectativas del proyecto.

### Actualización
Los datos se extraen en tiempo real para garantizar que estén actualizados y reflejen la situación actual.

## Características del Proyecto
- Obtención de noticias a través de News API.
- Obtención de temperatura y clima a través de OpenWeatherMap API.
- Obtención de tipo de cambio a través de ExchangeRate API.
- Validación de calidad de los datos obtenidos.

## Como ejecutar el proyecto: Instalación y Configuración

1. Clona este repositorio en tu máquina local:
    ```bash
    git clone https://github.com/tu_usuario/indicadores-de-calidad-de-datos.git
    ```

2. Instala las dependencias necesarias:
    ```bash
    pip install -r requirements.txt
    ```

3. Crea un archivo `.env` en la raíz del proyecto y añade tus claves API:
    ```bash
    NEWS_API_KEY=tu_clave_api_news
    WEATHER_API_KEY=tu_clave_api_weather
    EXCHANGE_API_KEY=tu_clave_api_exchange
    ```

4. Ejecuta el notebook de Jupyter para obtener los datos y realizar el análisis:
    ```bash
    jupyter notebook notebook.ipynb
    ```

**Nota**: Asegúrate de que el archivo `.env` esté en tu `.gitignore` para no subirlo accidentalmente a GitHub.

## Uso

Después de seguir los pasos de instalación, simplemente ejecuta el notebook de Jupyter. Este descargará los datos de las APIs, los procesará y validará la calidad de los datos de acuerdo con los indicadores establecidos.

## Contribución

1. Haz un fork de este repositorio.
2. Crea tu rama de características (`git checkout -b feature/nueva-caracteristica`).
3. Haz tus cambios.
4. Haz un commit de tus cambios (`git commit -am 'Añadir nueva característica'`).
5. Envía un pull request.

## Licencia

Este proyecto está licenciado bajo la Licencia UPC.


## Notas

- **No subas tu archivo `.env` a GitHub**. Asegúrate de que esté incluido en el archivo `.gitignore`.
