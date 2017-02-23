# Consul running in Docker on AWS

The Dockerfile in this repository builds an image that allows to run [Consul](https://consul.io) on AWS.
Upon running, it determines the host's IP address using the [EC2 Instance Metadata API](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-metadata.html)
and tells Consul to use that IP as advertising address.

This project is based on the [official Consul image for Docker](https://github.com/hashicorp/docker-consul).
Please refer to the change log for information about differences.
