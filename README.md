# reliza-docker-action

## About

GitHub Action to Build a Docker image, push it to the registry and submit the release metadata to RelizaHub.

## Usage

```yaml
steps:
- uses: relizaio/reliza-docker-action@1.1
  with:
    reliza_api_id: <api-id-obtained-from-relizahub>
    reliza_api_key: <api-key-obtained-from-relizahub>
    registry_username: <image-registry-username>
    registry_password: <image-registry-password>
    registry_host: <image-registry-host>
    image_namespace: <registry-namespace>
    image_name: <image-name>
```

## Inputs
The actions supports the following inputs:

- `reliza_api_id`: The project API ID obtained from RelizaHub.
- `reliza_api_key`: The project API Key obtained from RelizaHub.
- `registry_username`: Username for the image registry.
- `registry_password`: Password for the image registry.
- `registry_host`: Image registry host.
- `image_namespace`: "Namespace of the image on registry.
- `image_name`: "Name of the image.
- `path`: Path to the relative to root of the repo (default is '.').
- `dockerfile_name`: Name of the dockerfile (default is 'Dockerfile').
