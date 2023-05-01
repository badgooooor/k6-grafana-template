# template-k6-grafana-dashboard

Template for running performance test with k6, embedded with Grafana and Influx.

### Commands

```
docker compose up -d influxdb grafana
# Change "/scripts/http_basic_auth.js" to other k6 script
docker compose run --rm k6 run /scripts/http_basic_auth.js
```

Dashboard will be available at http://localhost:3000/d/k6/k6-load-testing-results
