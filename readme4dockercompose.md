# 1. Create data directories
mkdir -p data/{mysql,redis} logs/web

# 2. Configure environment
cp .env.example .env 
# Edit .env with your settings

# 3. Start application
docker-compose up -d --build

# 4. Verify all running
docker-compose ps

# 5. Open browser
# http://localhost:5000


## Endpoints


| Endpoint | Teaches |
|----------|---------|
| `/` | UI/UX, real-time dashboards |
| `/health` | Docker health checks, service monitoring |
| `/info` | Service discovery, multi-container communication |
| `/api/visits` | Persistence vs volatility, different storage |
| `/api/db-test` | Database integration, error handling |
| `/api/redis-test` | Caching, performance optimization |




