FROM python:3.10
# author keynezzz
# RUN apt-get update \
#     && apt-get install -y \
#     && rm -fr /var/lib/apt/lists/*
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1
WORKDIR /backend
COPY clickboard-be/. /backend/
RUN pip install -r requirements.txt

EXPOSE 8000
CMD [ "python","manage.py","runserver","0.0.0.0:8000" ]
