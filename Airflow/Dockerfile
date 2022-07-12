# First-time build can take upto 10 mins.

FROM apache/airflow:2.3.3

ENV AIRFLOW_HOME=/opt/airflow

USER root
RUN apt-get update -qq && apt-get install vim -qqq

USER airflow
COPY requirements.txt .
RUN pip install -r requirements.txt

SHELL ["/bin/bash", "-o", "pipefail", "-e", "-u", "-x", "-c"]

WORKDIR $AIRFLOW_HOME

USER $AIRFLOW_UID