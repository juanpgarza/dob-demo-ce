ARG ODOO_VERSION
FROM ghcr.io/tecnativa/doodba@sha256:175aefa719d752eac68166202d02c075194986c06f5e98b9152934356c52b9b3

USER root

# Creates missing 'cache' folder for PyAFIPws.
RUN mkdir -p /usr/local/lib/python3.8/site-packages/pyafipws/cache
RUN chown -R odoo:odoo /usr/local/lib/python3.8/site-packages/pyafipws/cache

RUN chown odoo:odoo /etc/ssl/openssl.cnf

USER odoo
