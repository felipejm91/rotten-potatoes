FROM python:3.11-rc
WORKDIR /app
COPY requirements.txt ./
RUN python -m pip install -r ./requirements.txt
COPY . ./
EXPOSE 5000
ENTRYPOINT ["gunicorn", "--workers=3", "--bind", "0.0.0.0:5000", "-c", "config.py", "app:app"]
