# Helium Compose

**Helium Compose is the Docker Compose configuration for the Helium CMS.**  
Helium Compose | [Helium Backend](https://github.com/freuwort/helium-backend) | [Helium Frontend](https://github.com/freuwort/helium-frontend) | [Helium Screens](https://github.com/freuwort/helium-screens)

## Startup
Example folder structure:
```
/app
├── /helium
└── /website
```

Helium for production from /app:
```bash
docker compose -f helium/compose.yml -f helium/compose.production.yml --env-file helium/.env up -d
```

Helium for production with custom website from /app:
```bash
docker compose -f helium/compose.yml -f helium/compose.production.yml -f website/compose.yml --env-file helium/.env up -d
```

## Security Vulnerabilities

If you discover a security vulnerability within the Helium Compose, please send an email to Alyx Freuwört via [contact@freuwort.com](mailto:contact@freuwort.com).  
We will address all security vulnerabilities promptly.

## License

Helium Compose is an open-source project licensed under the [MIT license](https://opensource.org/licenses/MIT).