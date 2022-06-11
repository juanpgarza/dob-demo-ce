ARG ODOO_VERSION
FROM ghcr.io/tecnativa/doodba:${ODOO_VERSION}-onbuild

USER root

# Creates missing 'cache' folder for PyAFIPws.
RUN mkdir -p /usr/local/lib/python3.8/site-packages/pyafipws/cache
RUN chown -R odoo:odoo /usr/local/lib/python3.8/site-packages/pyafipws/cache

RUN chown odoo:odoo /etc/ssl/openssl.cnf

USER odoo
