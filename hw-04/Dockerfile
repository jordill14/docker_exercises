FROM nginx:1.19.3

HEALTHCHECK --interval=45s --timeout=5s --start-period=15s --retries=2 CMD curl -f http://localhost:80 || exit 1


