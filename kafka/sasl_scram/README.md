# Kafka Docker Compose Setup

This folder contains a Docker Compose setup for running Apache Kafka with SASL/SCRAM authentication and TLS encryption. It also includes Kafka UI for easy management of the Kafka cluster.

## Getting Started

To get started with this Kafka setup, clone the repository and navigate to the directory containing the `kafka/sasl_scram/docker-compose.yml` file.

Ensure you have Docker and Docker Compose installed on your system, then run the following command to start the services:

```bash
docker-compose up -d
```

This will start Zookeeper, Kafka, and Kafka UI services in detached mode.

## Configuration

Before running the Docker Compose file, make sure to:

- Replace the placeholder paths in the volumes with the actual paths to your JKS and JAAS configuration files.
- Update the SASL credentials in the `docker-compose.yml` and `jaas.conf` files with your secure credentials.

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply [open an issue](https://github.com/finallyRaunak/DockerBazaar/issues/new) with the tag "enhancement".

Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Issues

If you encounter any issues or have any questions, please report them in the [issues](https://github.com/finallyRaunak/DockerBazaar/issues/) section of this repository. We encourage you to provide as much information as possible to help us understand and address your concerns.

## License

Distributed under the MPL-2.0 License. See `LICENSE` for more information.

## Contact

- [finallyRaunak](https://github.com/finallyRaunak/finallyRaunak?tab=readme-ov-file#contact-me)