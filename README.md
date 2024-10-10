
# Almacenamiento de Vectores con MongoDB y OpenAI Embeddings

Este proyecto demuestra cómo construir un sistema de almacenamiento de vectores utilizando MongoDB para almacenar documentos y los modelos de embeddings de OpenAI para una eficiente recuperación de información. El sistema aprovecha el framework LangChain para gestionar la carga de documentos, división de texto y consultas.

## Características

- **Carga de Documentos**: Utiliza `langchain_community` para cargar documentos PDF y JSON en el sistema de almacenamiento de vectores.
- **Generación de Embeddings**: Usa el modelo de embeddings de OpenAI para convertir el texto en vectores de alta dimensión.
- **Integración con MongoDB**: Almacena y recupera los vectores de los documentos y sus metadatos en MongoDB.
- **División de Documentos**: Divide textos largos en fragmentos manejables usando el divisor recursivo de caracteres de LangChain.

## Requisitos

- Python 3.8 o superior
- Una instancia de MongoDB
- Clave de API de OpenAI

## Configuración

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/tu-repo-aqui.git
   cd tu-repo-aqui
   ```

2. **Instalar dependencias:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configurar MongoDB:**
   Asegúrate de tener una instancia de MongoDB en funcionamiento y accesible. Actualiza la cadena de conexión de MongoDB en la parte correspondiente del código.

4. **Configurar la clave de API de OpenAI:**
   Configura tu clave de API de OpenAI como una variable de entorno:
   ```bash
   export OPENAI_API_KEY='tu-clave-api-aqui'
   ```

5. **Ejecutar el notebook:**
   Abre y ejecuta el notebook de Jupyter:
   ```bash
   jupyter notebook vector-store-mongoDB-openai.ipynb
   ```

## Uso

- **Cargar Documentos**: Carga archivos PDF o JSON en el sistema utilizando los cargadores de documentos incorporados de LangChain.
- **Generar Embeddings**: Utiliza los modelos de embeddings de OpenAI para transformar el texto en vectores.
- **Almacenar y Recuperar en MongoDB**: Los vectores y los metadatos relacionados se almacenan en MongoDB para su posterior recuperación y consulta.

## Personalización

- Puedes modificar la lógica de división de documentos o el modelo utilizado para la generación de embeddings según tus necesidades.
- Los nombres de la colección y la base de datos de MongoDB se pueden ajustar en el archivo de configuración.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.
