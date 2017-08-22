FROM continuumio/anaconda3

RUN conda install -y -c conda-forge cartopy feather-format matplotlib netCDF4 eofs &&\
  conda install -y scikit-learn xarray

RUN  pip install git+git://github.com/jdossgollin/jdgpy@master
