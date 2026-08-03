# fleet-router

Edge router for platform-hosted fleet agents. One wildcard custom domain
(`*.agents.turingplanet.ai`) attaches to this service; Caddy routes each
hostname to the matching member service over Railway private networking
(`<slug>.railway.internal`). The Caddyfile is the routing table — regenerated
from `agent-registry/deployments.yaml` by the deploy workflow (RFC 001 §5).
