FROM python:3.9

WORKDIR /dj

COPY ./dj /dj

RUN pip install -r /dj/requirements.txt

# ENV SECRET_KEY django-insecure-9m2%u2yq=+#)6c#^j7^1p+@mpiob-r)9ki+zrv%*ad779fz89l
# ENV DEBUG 1

RUN python manage.py migrate

EXPOSE 8000

CMD ["gunicorn", "--bind", "0.0.0.0:8000", "smart_home.wsgi"]