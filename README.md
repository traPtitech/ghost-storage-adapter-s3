# ghost-storage-adapter-s3

An s3 storage adapter for Ghost blogging platform.
Resizes images and caches it.

## Installation
```sh
npm i traPtitech/ghost-storage-adapter-s3
mkdir -p ./content/adapters/storage
cp -r ./node_modules/ghost-storage-adapter-s3 ./content/adapters/storage/s3
```

## Configuration
```json
{
  "storage": {
    "active": "s3",
    "s3": {
      "accessKeyId": "s3-access-key-id",
      "secretAccessKey": "s3-secret-access-key",
      "region": "your-region",
      "bucket": "your-bucket-name",
      "serverUrl": "your-page-domain/content/images",
      "endpoint": "your-s3-endpoint",
      "cacheFolder": "cache-folder-name"
    }
  },
  "imageOptimization": {
    "resize": false
  }
}
```
