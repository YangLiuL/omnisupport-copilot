FROM registry.cn-hangzhou.aliyuncs.com/library/python:3.11-slim

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -i https://pypi.tuna.tsinghua.edu.cn/simple -r requirements.txt

COPY ticket_simulator.py .

CMD ["python", "ticket_simulator.py", "--count", "500", "--output", "/data/tickets-seed-batch-001.jsonl"]
