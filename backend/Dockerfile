
#lite version form python 
FROM python:3.11-slim 

#worker folder
WORKDIR /app

#copy for all requirements and run the pip 
COPY requirements.txt .
RUN pip install --default-timeout=10000 --retries 20 --no-cache-dir -r requirements.txt


#then copy all file in APP folder  
COPY . .

# run in prot backend 5002
EXPOSE 5002

#code for run python 
CMD ["python", "app.py"]
