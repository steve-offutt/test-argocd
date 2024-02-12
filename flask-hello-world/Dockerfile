FROM python:3.12

RUN groupadd -r app
RUN useradd -r -u 1000 -g app app

WORKDIR /code
RUN chown -R app:app /code
COPY src .
RUN pip install -r requirements.txt
EXPOSE 5000
USER 1000
ENTRYPOINT [ "python3" ]
CMD [ "app.py" ]