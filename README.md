# sensAIhub-main
An integrated AI-driven system that combines computer vision, voice processing, and sensor data processing to create an intelligent and responsive environment.

## Overview

SensAIHub leverages various sensors and AI technologies to enable data-driven user interactions. By processing multiple streams of sensory data in real-time, the system can respond intelligently to user presence, actions, and inputs, creating a highly responsive and adaptive environment. Designed to run primarily on a Raspberry Pi, with additional processing capabilities provided by a backend GPU server, SensAIHub aims to push the boundaries of human-computer interaction.

## Key Concepts

- **Data-Driven Interaction**: Utilizes real-time sensor data to inform and enhance user interactions
- **Multimodal Sensing**: Combines visual, auditory, and environmental data for comprehensive user understanding
- **Adaptive Response**: Tailors system behavior based on analyzed user data and context
- **Edge Computing**: Balances local processing with cloud capabilities for efficient operation


## Features

- **Computer Vision**: Face detection, landmark tracking, head orientation, and gaze direction estimation using Google MediaPipe
- **Voice Processing**: Wake-word detection, speaker diarization, voice pitch estimation, and speech-to-text conversion
- **Conversational AI**: Integration with a small LLM (e.g., Llama or Geitje) for natural language interaction
- **Presence Detection**: Utilizes radar sensors for user presence, breathing rate, and potentially heart rate monitoring
- **Distributed Processing**: Local processing on Raspberry Pi with heavy computational tasks offloaded to a GPU server
- **Remote Development**: Supports remote development and debugging via Tailscale network


## System Architecture

- **Edge Device**: Raspberry Pi 4
- **Auxiliary MCU**: Raspberry Pi Zero (for low-level sensor integration)
- **Backend**: GPU server for intensive processing tasks
- **Network**: Tailscale VPN for secure remote access

## Development Setup

1. Set up Raspberry Pi with Raspberry Pi OS
2. Install Tailscale on all devices (Pi, development machine, server)
3. Configure VSCode with Remote-SSH extension for development
4. Clone this repository and its submodules

Detailed setup instructions can be found in the [docs/setup.md](docs/setup.md) file.

## Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for more details.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

This project makes use of several open-source libraries and tools. We thank all the contributors to these projects.

## Contact

For any queries regarding this project, please open an issue in this repository.
