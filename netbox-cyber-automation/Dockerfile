FROM docker.io/netboxcommunity/netbox:v4.4-3.4.1

# Copy plugin requirements into the image
COPY ./plugin_requirements.txt /opt/netbox/

# Install plugins into NetBox's venv using uv
RUN /usr/local/bin/uv pip install -r /opt/netbox/plugin_requirements.txt
