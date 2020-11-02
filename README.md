# Lokdhaba-API-dj
API to fetch data from LokDhaba

The following needs to be included in the docker compose files
'''

  web:
    build: ./Lokdhaba_dj
    container_name: ld_dj
    command: python manage.py runserver 0.0.0.0:8000
    volumes:
    - './Lokdhaba_dj/:/app/'
    ports:
    - "8000:8000"
    links :
    - db

'''
