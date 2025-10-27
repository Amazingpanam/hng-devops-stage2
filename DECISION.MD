Nginx serves as a reverse proxy routing traffic between two Node.js containers — Blue and Green. It supports automatic failover using Nginx’s backup directive and Docker health checks to detect unhealthy instances.

The decision were based on the following below

1. Dynamic templating: envsubst enables switching environments via ACTIVE_POOL without editing configs.
2. Health checks: Improve reliability and allow smoother failover during CI tests.
3. Timeouts & retries: Tuned to meet the 10-second failover requirement.
4. Parameterization: All variables are managed through the .env file for consistent automation.

The results

1. Zero-downtime switching
2. Reliable failover
3. ully parameterized, reproducible setup
