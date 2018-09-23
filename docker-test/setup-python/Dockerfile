FROM python:3.7.0

WORKDIR /test
ADD . /test
RUN pip install --trusted-host pypi.python.org -r requirements.txt
EXPOSE 1111
ENV name this_name
CMD ["python","app.py"]