FROM python:3.9.10

# add all necessary files for the project
ADD . /app/

# go into container work directory
WORKDIR /app

# install all dependancies needed for app good running
RUN pip install --no-cache-dir -r requirements.txt

# Expose app entry with port 8501
EXPOSE 8501

# Command for running streamlit app
CMD ["streamlit", "run", "streamlit_dashboard_app.py", "--server.port=8501"]
