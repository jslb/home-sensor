FROM grafana/grafana:8.2.3-ubuntu

# Disable Login form or not
ENV GF_AUTH_DISABLE_LOGIN_FORM "false"
# Allow anonymous authentication or not
ENV GF_AUTH_ANONYMOUS_ENABLED "true"
# Role of anonymous user
ENV GF_AUTH_ANONYMOUS_ORG_ROLE "Admin"
# Install plugins, comma separated
ENV GF_INSTALL_PLUGINS="yesoreyeram-infinity-datasource"

# Add provisioning
ADD ./provisioning /etc/grafana/provisioning
# Add configuration file
ADD ./grafana.ini /etc/grafana/grafana.ini
# Add dashboard json files
ADD ./dashboards /etc/grafana/dashboards
