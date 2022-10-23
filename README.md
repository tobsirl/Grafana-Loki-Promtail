# Grafana-Loki-Promtail

## Notes on Introduction to Loki: Like Prometheus, but for Logs

[Introduction to Loki: Like Prometheus, but for Logs](https://grafana.com/go/webinar/intro-to-loki-like-prometheus-but-for-logs/)

## What is Loki?

- Loki is an Apache 2.0 licensed log aggregation system inspired by Prometheus. It is designed to be very cost effective and easy to operate. It does not index the contents of the logs, but rather a set of labels for each log stream.

## What is Promtail?

- Loki **does not index the text of the logs,** instead grouping entries into **streams** and indexing those with **labels.**
- This is mainly due to cost and performance reasons. Indexing the text of the logs would be very expensive and slow.
- Unlike Prometheus, Promtail doesn’t pull logs
- Prometheus scrapes logs for you
- Same scrape config with Prometheus can be used promtail, same labels for metrics and logs
- promtail - syslog through TCP

## How does it work?

![How does it work](/images/howdoesitwork.PNG)

### Understanding the Loki model

![Logs](/images/logs.PNG)
![Streams](/images/streams.PNG)
![Chunks](/images/chunks.PNG)
![Query](/images/query.PNG)

## Labels

![Query](/images/labels.PNG)
![Query](/images/loglines.PNG)

## How do I query without an index?

![Query](/images/index.PNG)

## LogQL

![Query](/images/logql.PNG)
