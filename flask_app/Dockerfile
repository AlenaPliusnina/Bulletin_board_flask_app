FROM python:3.7

EXPOSE 5000

WORKDIR /flask_app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD [ "python", "./app.py" ]