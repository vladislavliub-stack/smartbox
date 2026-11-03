# SmartBox

ESP32 smart workshop controller, Telegram bot and Jarvis voice assistant.

- [Firmware, Telegram and MQTT setup](SmartBoxProject-main/README.md)
- [Jarvis setup](Jarvis-main/README.md)

The archive's source folders are preserved. Real `.env` files, runtime configuration,
build outputs, cached dependencies and bytecode are excluded from this repository.
Configuration examples contain only placeholders or empty credentials.

Create `SmartBoxProject-main/firmware/include/config.h` from `config_example.h`,
and each application's `.env` from its `.env.example`. Set your own credentials locally.
Never force-add ignored configuration or broker password files.

Start Mosquitto from `SmartBoxProject-main` with its `mosquitto/mosquitto.conf`.
Create the three local MQTT accounts as described in the setup guide.

Run `python -m unittest discover -s tests` inside each source folder.
Firmware compilation requires PlatformIO and a local `config.h`; device operation
requires the ESP32, sensors, broker and application dependencies.
