# Google Cloud Cheatsheet

Google Cloud is a cloud computing platform that provides a wide range of services and tools for building and deploying applications. Here is an overview of some of its basic syntax and features.

## Compute Engine

### Creating an instance
```
gcloud compute instances create my-instance --image-family=debian-10 --image-project=debian-cloud --machine-type=n1-standard-1 --zone=us-central1-a
```

### Stopping an instance
```
gcloud compute instances stop my-instance --zone=us-central1-a
```

### Starting an instance
```
gcloud compute instances start my-instance --zone=us-central1-a
```

## Cloud Storage

### Creating a bucket
```
gsutil mb gs://my-bucket-name/
```

### Uploading a file
```
gsutil cp /path/to/local/file gs://my-bucket-name/path/to/gs/file
```

### Downloading a file
```
gsutil cp gs://my-bucket-name/path/to/gs/file /path/to/local/file
```

## Cloud Functions

### Creating a function
```
gcloud functions deploy my-function --runtime python38 --trigger-http --entry-point my_function --allow-unauthenticated
```

### Invoking a function
```
gcloud functions call my-function --data '{"key1": "value1", "key2": "value2", "key3": "value3"}'
```

## Resources

- [Google Cloud Documentation](https://cloud.google.com/docs)
- [Google Cloud SDK Command Reference](https://cloud.google.com/sdk/docs/command-reference)