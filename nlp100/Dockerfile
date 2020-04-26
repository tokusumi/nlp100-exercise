FROM tensorflow/tensorflow:2.1.0-py3-jupyter

RUN apt-get update && \
    apt-get install git -y
RUN python -m pip install pip --upgrade

RUN python -m pip install jupyter_contrib_nbextensions jupyter_nbextensions_configurator && \
    jupyter contrib nbextension install --user && \
    jupyter nbextensions_configurator enable --user

WORKDIR /notebooks
ADD requirements.txt /notebooks/requirements.txt

RUN python -m pip install -r requirements.txt
COPY . /notebooks