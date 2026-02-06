# ESPHome Development Resources

This file contains a collection of resources to help you with ESPHome development.

## Official Documentation

*   **ESPHome Website:** [https://esphome.io/](https://esphome.io/) - The official website is the best place to start.
*   **Getting Started Guide:** [https://esphome.io/guides/getting_started_command_line.html](https://esphome.io/guides/getting_started_command_line.html)
*   **Components Index:** [https://esphome.io/components/](https://esphome.io/components/) - A full list of all official components.

## Community & Support

*   **ESPHome Discord:** [https://discord.gg/KhAMkrd](https://discord.gg/KhAMkrd) - A very active community for help and sharing projects.
*   **Home Assistant Community:** [https://community.home-assistant.io/c/esphome/](https://community.home-assistant.io/c/esphome/)

## Useful Tools

*   **ESPHome-Flasher:** [https://github.com/esphome/esphome-flasher/releases](https://github.com/esphome/esphome-flasher/releases) - A GUI tool for flashing ESPHome firmware.
*   **YAML Validator:** [https://www.yamllint.com/](https://www.yamllint.com/) - A web-based tool for checking your YAML syntax.

## Example Configuration

Here is a very basic example of a `m5-dial.yaml` file for an M5Dial, which turns on a web server so you can see the logs.

```yaml
esphome:
  name: m5-dial
  friendly_name: M5 Dial

esp32:
  board: m5stack-dial
  framework:
    type: arduino

# Enable the web server so you can view logs
web_server:
  port: 80

# Enable logging
logger:

# Enable API for Home Assistant
api:
```