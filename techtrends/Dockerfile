FROM python:3.8
LABEL maintainer="Abhirup Sarkar"

COPY . /app
WORKDIR /app
RUN pip install -r ./techtrends/requirements.txt
RUN python ./techtrends/init_db.py
EXPOSE 3111
# command to run on container start
CMD [ "python", "./techtrends/app.py" ]
