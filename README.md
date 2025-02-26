# Guide to connect elasticsearch in mongodb, and schedule sync data.

## Create an  MongoDb connector:
![image](https://github.com/user-attachments/assets/05915bfe-870c-400c-b826-f3175ddac57f)
![image](https://github.com/user-attachments/assets/306cf28c-4911-448c-92c8-aa2ca3c0768b)



## Setup your config.yml with data provided in elasticsearch connectors pannel:
```yml
connectors:
-
  connector_id: connector_id
  service_type: mongodb
  api_key: api_key
elasticsearch:
  host: host
  api_key: api_key
```

## Run from docker, in or own infrastructure:

```
docker compose up -D connector
```

## In elasticsearch pannel, check if the connection is successful:
![image](https://github.com/user-attachments/assets/7edec2ed-2c6b-428a-9450-07c89abf1ea3)

### If you're using atlas, enable tls connection:
![image](https://github.com/user-attachments/assets/488b5b87-7e06-4dac-878b-5fcc61574215)

## Fill the required connection params, and click in "Save":
![image](https://github.com/user-attachments/assets/75cec3bb-a480-4a38-8247-1bc0cc1ced91)

## Connect and index, and click in "Save and Sync":
![image](https://github.com/user-attachments/assets/e271cbcc-b4a3-42bd-9e85-d64519494226)

## Now, you can see the failed or successfully syncs:
![image](https://github.com/user-attachments/assets/01abb658-2d7c-47ad-bf25-23ce7baf59bd)



