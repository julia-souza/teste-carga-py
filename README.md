# Teste de carga utilizando Locust
![Badge em Desenvolvimento](https://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge) 
![Python](https://forthebadge.com/images/badges/made-with-python.svg)
![lOCUST](/img/locust.svg)
![4test](/img/test.svg)
![BUILD](https://forthebadge.com/images/badges/built-with-love.svg)

## Preparando o ambiente

Requer Python 3.7, FastAPI e Locust 

Instalar as dependências:

```sh
cd C:\wamp64\www\projetos\_estudos\teste-carga
pip install fastapi
pip install "uvicorn[standard]"
pip install locust
```

Para executar a aplicação teste

```sh
uvicorn main:app --reload
```

Para executar o teste

```sh
locust --headless --users 10 --spawn-rate 1 -H http://127.0.0.1:8000
```

Locust executa na porta 8089 
(http://localhost:8089)