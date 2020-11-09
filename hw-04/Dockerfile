FROM nginx:1.19.3

RUN apt-get update && apt-get install -y wget

EXPOSE 8080

HEALTHCHECK --interval=45s --timeout=5s --start-period=15s --retries=2 CMD curl -f http://localhost:8080 || exit 1


