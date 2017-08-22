FROM continuumio/miniconda3

RUN conda install -y argparse calendar datetime jupyter matplotlib numpy pandas scikit-learn xarray

RUN conda install -y -c conda-forge cartopy feather-format netCDF4 eofs

RUN  pip install git+git://github.com/jdossgollin/jdgpy@master
