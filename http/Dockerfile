FROM openpolicyagent/opa:latest


COPY auth.rego /etc/opa/bundles/auth.rego
COPY hr.rego /etc/opa/bundles/hr.rego

CMD ["run", "--log-level=debug", "--server", "--log-format=json-pretty", "--set=decision_logs.console=true", "/etc/opa/bundles/auh.rego"]
