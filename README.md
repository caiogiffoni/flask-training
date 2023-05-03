# flask-training

build image
docker build -t flask-smorest-api .

build container
docker run -d -p 5000:5000 rest-apis-flask-python

build container
docker run -dp 5000:5000 -w /app -v "$(pwd):/app" flask-smorest-api



how to create db and migrations:
flask db init

flask db migrate

flask db upgrade




run locally
docker run -dp 5000:5000 -w /app -v "$(pwd):/app" teclado-site-flask sh -c "flask run --host 0.0.0.0"

hello test