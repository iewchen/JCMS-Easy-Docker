FROM python:2.7-stretch

ADD . /var/webapp/flask-jcmsui
WORKDIR /var/webapp/flask-jcmsui

RUN pip install -r requirements.txt

# install latex
RUN apt-get update -q && apt-get install -qy \
    texlive-full \
    python-pygments gnuplot \
    make git \
	&& rm -rf /var/lib/apt/lists/*


CMD python jcmsui.py
