# Reliability

The biggest improvement I'd make to the reliability of this system
would be to use configuration management such as Ansible.

If configured correctly, it should be easy to recommission the server
into a consistent state.

I would also consider containerizing the running services to simpify upgrades
and enable easier testing.

I would also consider using a tool like `yum-cron` for automated security
updates. Alongside a monthly manual upgrade schedule to ensure packages are
kept up to date.

Finally, I would look into a centralized logging and monitoring, for example
Prometheus/Grafana/Loki to ensure any issues are quickly identified, alerted on,
and resolved.