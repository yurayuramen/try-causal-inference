FROM jupyter/datascience-notebook:lab-3.0.5

USER root

RUN apt-get update && apt-get install fonts-noto-cjk

USER jovyan

RUN R -e "install.packages('haven', repos='https://cran.ism.ac.jp')"

RUN pip --use-deprecated=legacy-resolver install pycaret[full]==2.3.2 shap==0.37.0 econml==0.11.1 causalml==0.10.0 optuna==2.8.0

