# Linode Cheatsheet

Linode is a cloud computing platform that provides a wide range of services and tools for building and deploying applications. Here is an overview of some of its basic syntax and features.

## Instances

### Creating an instance
```
linode-cli linodes create --type g6-nanode-1 --region us-east --image linode/ubuntu20.04 --root-pass password --authorized-keys-file /path/to/public/key
```

### Booting an instance
```
linode-cli linodes boot 12345
```

### Shutting down an instance
```
linode-cli linodes shutdown 12345
```

## Object Storage

### Creating a bucket
```
linode-cli objects create-bucket --cluster us-east --label my-bucket-name
```

### Uploading a file
```
linode-cli objects put my-bucket-name /path/to/local/file /remote/path/file
```

### Downloading a file
```
linode-cli objects get my-bucket-name /remote/path/file /path/to/local/file
```

## Kubernetes

### Creating a cluster
```
linode-cli k8s-alpha create my-cluster --region us-east --node-pool "type=g6-standard-2;count=3;label=web" --version 1.21
```

### Scaling a cluster
```
linode-cli k8s-alpha node-pool-scale my-cluster web 5
```

## Resources

- [Linode Documentation](https://www.linode.com/docs/)
- [Linode CLI Reference](https://www.linode.com/docs/guides/linode-cli-reference/)