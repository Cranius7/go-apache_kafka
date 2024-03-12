# go-apache_kafka
# High Availability Microservice with Apache Kafka using Golang

This repository contains a high availability microservice built with Golang, which utilizes Apache Kafka for message queuing.

## Setup

1. **Requirements**: Ensure you have Go 1.11 or higher, Apache Kafka, and the `confluent-kafka-go` library installed.

2. **Installation**:
   - Clone the repository:
     ```
     git clone https://github.com/Cranius7/go-apache_kafka.git
     ```

3. **Build and Run**:
   - Build the Go program:
     ```
     go build main.go
     ```
   - Run the compiled program:
     ```
     ./main
     ```

## Code Overview

- `main.go`: Contains the main functionality of the microservice.
- The `OrderPlacer` struct manages the Kafka producer and facilitates order placement.
- Each order is produced asynchronously to Kafka, and a delivery channel is used to track the delivery status.
- The `main()` function sets up the Kafka producer, initializes the `OrderPlacer`, and places orders with a simulated delay of 3 seconds between each order.

## Repository Structure

- **main.go**: Contains the main Go code for the microservice.
- **README.md**: Instructions and documentation for setting up and running the microservice.


## Contributions and Issues

- Contributions to enhance the microservice are welcome via pull requests.
- For any issues encountered while using the microservice, please open an issue on GitHub.

## License

This microservice is licensed under the [MIT License](LICENSE).

For any further inquiries or assistance, feel free to contact the repository owner.

Thank you for using our microservice!
