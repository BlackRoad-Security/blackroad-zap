# 🚀 BlackRoad Deployment Guide

## Quick Start

### Using Docker Compose (Recommended)

```bash
# Start the service
docker-compose -f docker-compose.blackroad.yml up -d

# View logs
docker-compose -f docker-compose.blackroad.yml logs -f

# Stop the service
docker-compose -f docker-compose.blackroad.yml down
```

### Using BlackRoad Infrastructure

This service integrates with the complete BlackRoad OS ecosystem:

1. **Monitoring**: Automatic Prometheus + Grafana integration
2. **Logging**: Centralized logging to BlackRoad ELK stack
3. **Security**: Integrated with BlackRoad Security division
4. **Networking**: Connects to blackroad-network overlay
5. **Storage**: Backed up to BlackRoad Archive systems

## Configuration

All BlackRoad services use environment variables for configuration:

- `BLACKROAD_ORG`: Organization (auto-set)
- `BLACKROAD_MANAGED`: Managed by BlackRoad (auto-set to true)
- `TZ`: Timezone (default: America/Chicago)

## Production Deployment

For full production deployment:

1. Review `docker-compose.blackroad.yml`
2. Configure environment variables in `.env`
3. Set up SSL/TLS certificates (see BlackRoad-Security)
4. Enable monitoring (see BlackRoad-OS/monitoring)
5. Configure backups (see BlackRoad-Archive)

## Support

- Issues: File in this repository
- BlackRoad Infrastructure: https://github.com/BlackRoad-OS
- Email: blackroad.systems@gmail.com

---

**BlackRoad OS, Inc. - Digital Sovereignty Infrastructure**
