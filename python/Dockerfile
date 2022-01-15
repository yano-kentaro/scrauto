FROM python:3.9.6

RUN pip install --upgrade pip
RUN pip install jupyterlab
RUN pip install selenium
RUN pip install requests

WORKDIR /JupyterLab

EXPOSE 8888

ENTRYPOINT ["jupyter-lab", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root", "--NotebookApp.token=''"]

CMD ["--notebook-dir=/JupyterLab"]