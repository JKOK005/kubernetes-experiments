FROM python:3
WORKDIR /setup-full-pip-installation
ADD requirements.txt pip-install/ 
ADD app.py runnable/

RUN pip install --trusted-host pypi.python.org -r pip-install/requirements.txt

#EXPOSE 7000
CMD ["python", "runnable/app.py"]