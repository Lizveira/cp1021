FROM python:3.11-slim
LABEL maintainer="Elizandra <lizveiragues@gmail.com>" 
LABEL description="Aplicação Python com Flask"
LABEL version="1.0.0"
Workdir /app
COPY . . 
RUN pip install --no-cache-dir -r requeriments.txt

RUN useradd -m appuser
USER appuser


EXPOSE 5000
CMD ["python", "app.py"]