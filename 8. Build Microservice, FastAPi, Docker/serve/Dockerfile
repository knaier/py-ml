FROM tiangolo/uvicorn-gunicorn-fastapi:latest
COPY ./requirements.txt /opt/app/requirements.txt
WORKDIR /opt/app
RUN pip install --no-cache-dir --upgrade -r requirements.txt
COPY ./src /opt/app
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8081"]
# docker docker build -t knaier/custom-forecasting-service:latest .
# docker login
# docker push knaier/custom-forecasting-service:latest
# run via