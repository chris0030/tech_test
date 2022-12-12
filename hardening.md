# Hardening the system

My approach for hardening this system would be to use an opinionated 
and objective framework to enable me to repeatedly and consistently secure
the server. This would ideally use configuration management tools such as 
Ansible to keep the configuration applied.

With this in mind, I'd consider something like the following https://dev-sec.io/
taking advantage of their configuration templates for Ansible to automate the
hardening of the server. 

In the meantime, I'd ensure at least the following is done.

* Root account should be locked down, not able to be SSH'd into
* Consider using a VPN or bastion host to control/audit/log access to the server
* Postgres needs hardening with passwords/default accounts removed
* SSH Config needs reviewing to ensure keys are required for access
* Remote logging/monitoring/alerting need to be considered
* Consider an AWS Inspector security agent (costs need considering)
* Consider a WAF or ALB infront of the instance for added security
* Ensure any unused services are removed or disabled
* Ensure any unused ports are closed