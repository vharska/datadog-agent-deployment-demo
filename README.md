# datadog-agent-deployment-demo
automating the deployment of the Datadog agent.

# Check syntax
ansible-playbook playbooks/deploy_datadog.yml --syntax-check

# Test with specific environment (dry-run)
ansible-playbook playbooks/deploy_datadog.yml --limit dev --check

# Deploy to specific environment
ansible-playbook playbooks/deploy_datadog.yml --limit dev
This implementation automatically configures the Datadog agent with appropriate settings for each environment, collects logs, and sets up various integrations based on the environment.
