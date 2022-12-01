# Metrics Consumer

Internally the ez-python-autotyper has an event queue. Metrics consumers will read those events and persist them to
a `metrics.json` file. A metrics consumer is created for jobs by default unless specified otherwise via the
boolean `COLLECT_METRICS` field in its corresponding `job spec`.