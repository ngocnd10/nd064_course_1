FROM python:3.8
LABEL maintainer="Ngoc Nguyen"

COPY ./project/techtrends /app
WORKDIR /app
RUN pip install -r requirements.txt

# command to init database
RUN python init_db.py

EXPOSE 3111

# command to run on container start
CMD [ "python", "app.py" ]
