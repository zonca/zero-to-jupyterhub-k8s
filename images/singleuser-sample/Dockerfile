FROM jupyter/datascience-notebook:281505737f8a

# conda/pip/apt install additional packages here, if desired.

# pin jupyterhub to match the Hub version
# set via --build-arg in Makefile
ARG JUPYTERHUB_VERSION=0.8
RUN pip install --upgrade --no-deps https://github.com/zonca/jupyterhub/archive/fix_cookie_cilogon.zip jupyterlab

RUN jupyter serverextension enable --py jupyterlab --sys-prefix
#RUN jupyter labextension install @jupyterlab/hub-extension
