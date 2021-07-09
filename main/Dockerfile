FROM python:3.8.0

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        postgresql-client \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir /main
WORKDIR /main/

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN pip3 install torch torchvision torchaudio
COPY . /main/

EXPOSE 8000
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]