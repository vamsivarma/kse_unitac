FROM jupyter/base-notebook:latest

RUN mamba install -c conda-forge leafmap geopandas localtileserver -y && \
    fix-permissions "${CONDA_DIR}" && \
    fix-permissions "/home/${NB_USER}"

COPY requirements.txt .
RUN pip install -r requirements.txt

RUN mkdir ./pages
COPY /pages ./pages

RUN mkdir ./template
COPY /template ./template

RUN mkdir ./data
COPY /data ./data

ENV PROJ_LIB='/opt/conda/share/proj'

USER root
RUN chown -R ${NB_UID} ${HOME}
USER ${NB_USER}

EXPOSE 8765

# You can also run apps under pages here by replacing ./template with ./pages
CMD ["solara", "run", "./template", "--host=0.0.0.0"]
