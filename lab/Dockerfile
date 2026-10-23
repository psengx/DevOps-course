FROM python:3.13-slim-bookworm
WORKDIR /app
ENV PYTHONUNBUFFERED=1 PYTHONDONTWRITEBYTECODE=1
COPY app.py index.html ./
RUN mkdir /data && chown 10001:10001 /data
LABEL course.student="06052007"
USER 10001:10001
EXPOSE 8000
CMD ["python", "app.py"]
