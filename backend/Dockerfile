FROM python:3.12-slim
WORKDIR /backend
COPY requirements.txt /backend
RUN pip3 install --upgrade pip -r requirements.txt
COPY . /backend
EXPOSE 5000
ENV FLASK_APP=main.py
CMD ["flask", "run", "--host=0.0.0.0"]