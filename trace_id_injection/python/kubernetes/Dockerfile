# syntax=docker/dockerfile:1

FROM python:3.9.14-slim

WORKDIR /app

RUN pip3 install ddtrace json_log_formatter

COPY trace_id_injection.py /app

CMD ["ddtrace-run", "python3", "trace_id_injection.py"]
