FROM python:3.8

WORKDIR /usr/src/app

COPY ./project/techtrends/requirements.txt ./

RUN pip3 install --no-cache-dir -r requirements.txt

COPY ./project/techtrends ./

RUN python3 init_db.py

EXPOSE 3111

CMD ["python3", "app.py"]