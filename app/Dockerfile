FROM python:3.10-slim

WORKDIR /app

COPY python/requirements.txt .

RUN pip3 install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 8501

CMD ["streamlit", "run", "python/Chatbot.py", "--server.port=8501", "--server.address=0.0.0.0"]
