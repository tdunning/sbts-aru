## StalkedByTheState: Autonomous Recording Unit 

Welcome to the autonomous recording unit enhancement of the **StalkedByTheState** security suite.

### Introduction:
While initially conceived to augment security, this module serves a dual purpose. It introduces the concept of an **Autonomous Recording Unit (ARU)**, a term prominently used in bioacoustics. What sets this ARU apart is its ability to precisely synchronize the time of arrival for audio packets and it installs on cheap raspberry pi hardware. Coupled with a tracking file, this enables pinpoint **Time Difference of Arrival (TDOA) sound localization**.

### Key Features:

1. **GPS and PPS Integration:** To ensure unmatched precision, the project is optimized to function on a computer that integrates with a GPS. By utilizing the Pulse Per Second (PPS) interrupt, it aligns system time typically to sub-microsecond accuracy.
   
2. **Time Synchronization:** By initiating a clap near co-located microphones running `sbts-aru`, users can align the clap's time with the actual time. The typical alignment error margin from the waveforms from the sound files is under 1ms. Given that sound covers approximately 34cm in 1ms, this ensures high effective sound localization, even over short distances.

### Potential Use Cases:
- **Bioacoustic Studies:** This technology can be instrumental for researchers aiming to localize various species based on their vocalizations or other sound signatures.

### Setup Instructions

1. **First**
2. Configure local settings

```
sudo raspi-config
```
Configure the following local settings
- Interface Options/SSH
- Localisation Options/Locale
- Localisation Options/Timezone
- Localisation Options/Keyboard
- Localisation Options/WLAN Country

If you have questions or feedback, don't hesitate to  reach out.
