# OM2M

This repository contains the official OM2M source code. I am not the author, and all rights belong to their respective owners.

## Why This Repository?

The original OM2M repository is currently unavailable for download. To ensure accessibility for research and development purposes, I have uploaded the source code here. This repository serves as a backup for those who need OM2M for IoT and oneM2M-based applications.

## About OM2M

OM2M is an open-source implementation of the oneM2M standard, designed to provide interoperability between IoT devices and applications. It enables:
- M2M communications using the oneM2M standard
- Secure and scalable IoT deployments
- Support for multiple communication protocols

## Installation

To set up OM2M, follow these steps:

1. Clone the repository:
   ```bash
   git clone <your-repo-link>
   ```
2. Navigate to the project directory:
   ```bash
   cd om2m
   ```
3. Run the appropriate script:
   ```bash
   ./start.sh   # For Linux/Mac
   start.bat    # For Windows
   ```

## Requirements

- Java 8 (OM2M runs only on Java 8)

## Usage

Once OM2M is running, you can:
- Access the Web UI at `http://localhost:8080/webpage`
- Use REST APIs for managing resources
- Connect IoT devices following oneM2M specifications

## Posting Data to OM2M via MQTT

To post data to OM2M using MQTT, you can use the [MQTT-OM2M Data Posting](https://github.com/likhithkanigolla/MQTT-OM2M) scripts.

### Steps

1. Ensure OM2M is running (see installation instructions above).
2. Clone the MQTT-OM2M helper repository:
   ```
   git clone https://github.com/likhithkanigolla/MQTT-OM2M.git
   cd MQTT-OM2M
   ```
3. Install Python dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Start the MQTT broker:
   ```
   python mqtt_broker.py
   ```
5. Run the test client to post data:
   ```
   python mqtt_test_client.py
   ```

This will publish sample data to OM2M using MQTT, demonstrating how IoT devices can interact with OM2M via the MQTT protocol.

For more details, see the [MQTT-OM2M Data Posting repository](https://github.com/likhithkanigolla/MQTT-OM2M).


## Disclaimer

This repository is provided as-is for accessibility purposes. I do not claim ownership of OM2M, and all rights remain with the original authors and maintainers.

## License

Refer to the original OM2M license terms for legal usage and distribution policies.

