# Dockerfile for Grafana
FROM grafana/grafana:9.1.2

# Expose port 3000
EXPOSE 3000

# Copy datasource and dashboard configurations
COPY ./datasources/all.yml /etc/grafana/provisioning/datasources/all.yml
COPY ./dashboards/all.yml /etc/grafana/provisioning/dashboards/all.yml
COPY ./krakend /var/lib/grafana/dashboards/krakend
