## Entrega 1

Para correr el script `Entrega1_FabioLecce.ipynb` se debe ejecutar el docker-compose que contiene el contenedor de Pyspark con Jupyter Notebook.
(Usando la misma configuracion que se levanto en el docker del ejemplo)

## Docker Compose con Pyspark
(Crear una imagen de Pyspark en el Docker)
```bash
docker-compose -f ./Entrega_1/docker-compose.yml up --build
```

> Password o Token del Jupyter Notebook: `coder`

> URL del Jupyter Notebook: [http://localhost:8888/lab?token=coder](http://localhost:8888/lab?token=coder)

## Archivo con claves Redshift

Hay que crear un archivo llamado `.env` con las siguientes claves:

```bash
AWS_REDSHIFT_USER=your-user
AWS_REDSHIFT_PASSWORD=your-password
AWS_REDSHIFT_HOST=data-engineer-cluster.cyhh5bfevlmn.us-east-1.redshift.amazonaws.com
AWS_REDSHIFT_PORT=5439
AWS_REDSHIFT_DBNAME=data-engineer-database
AWS_REDSHIFT_SCHEMA=your-schema
```

Y colocarlo en la carpeta `Entrega_1/docker_shared_folder/working_dir/`
