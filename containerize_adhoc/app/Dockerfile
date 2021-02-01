# your code goes here ...

FROM python:3.7.5-alpine


# RUN apk update && apk add bash

# Set the application directory
# RUN mkdir /src
WORKDIR /src

COPY ./src/requirements.txt requirements.txt

# Install our requirements.txt
# ADD ./src .
# ADD ./scr/requirements.txt requirements.txt 
RUN pip install -r requirements.txt

# COPY ./src .

# ADD ./src/server.py server.py

EXPOSE 8000

# CMD ["gunicorn", "wsgi:app", "-b", "0.0.0.0:8000" --reload]

# CMD ["flask", "run", "--host=0.0.0.0", "--port=8000"]
