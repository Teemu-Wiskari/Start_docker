FROM python:3.10

WORKDIR /src
COPY ./requirements.txt /src/requirements.txt
RUN pip install --no-cache-dir --upgrade -r requirements.txt 

COPY . .
EXPOSE 6060

RUN python manage.py migrate
RUN python manage.py collectstatic --noinput 

CMD ["gunicorn", "--bind", "0.0.0.0:6060", "--workers", "3", "stocks_products.wsgi:application"]

