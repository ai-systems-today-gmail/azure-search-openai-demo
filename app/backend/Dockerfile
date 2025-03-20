FROM python:3.11-bullseye

WORKDIR /app

COPY ./ /app

# RUN python -m pip install gunicorn
RUN python -m pip install -r requirements.txt

EXPOSE 8000


CMD ["python3", "-m", "gunicorn", "-b", "0.0.0.0:8000", "main:app"]
