FROM python:3.10-slim

WORKDIR /app

COPY llm-examples/requirements.txt .

RUN pip3 install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 8501

CMD ["streamlit", "run", "llm-examples/Chatbot.py", "--server.port=8501", "--server.address=0.0.0.0"]
