# Grafana-Loki-Promtail

## Notes on Introduction to Loki: Like Prometheus, but for Logs

[Introduction to Loki: Like Prometheus, but for Logs](https://grafana.com/go/webinar/intro-to-loki-like-prometheus-but-for-logs/)

- Loki **does not index the text of the logs,** instead grouping entries into **streams** and indexing those with **labels.**
- This is mainly due to cost and performance reasons. Indexing the text of the logs would be very expensive and slow.
- 

