# Intensive Load Nginx K8s Cache Proxy

This project was designed to make use of an available Kubernetes infrastructure to provide a proxy server that makes cache of intensive read resources when a WAF or other device is not available.

The project is composed of two subprojects which deal with the creation of the required infrastructure (portal-infra-nginx) which is supposed to happen occasionally, and the creation of a Docker image to be deployed as the proxy that caches the static contents of a website (portal-frontend-nginx).

Currently the pipeline is implemented with azure pipelines, but it can be easily moved to any other pipeline technology.
