FROM python:3.8

EXPOSE 3111

COPY techtrends/requirements.txt ./
RUN pip install -r requirements.txt

WORKDIR /workspace/techtrends
ADD . /workspace
RUN python init_db.py

CMD ["python", "app.py"]
