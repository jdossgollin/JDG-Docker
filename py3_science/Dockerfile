FROM continuumio/miniconda3

RUN conda install -y numpy scipy matplotlib ipython jupyter pandas sympy nose

RUN conda install -y -c conda-forge cartopy feather-format netCDF4 eofs &&\
  conda install -y scikit-learn xarray

RUN  pip install git+git://github.com/jdossgollin/jdgpy@master
