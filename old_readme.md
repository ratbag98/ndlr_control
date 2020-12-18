# NDLR Control Modules for Max for Live

## Abstract

Provide controls for all the CCs mentioned in Appendix A of the [NDLR's User
Manual](https://conductivelabs.com/wp-content/uploads/2020/02/The-NDLR-User-Manual-v1.7.pdf) updated to the latest working firmware (1.1.071) at the time of writing.

## Setup

Create MIDI track with MIDI To set to the NDLR's "NDLR Cntl" channel.

Create MIDI track with MIDI From set to NDLR (Port 2), and the same channel.

## Notes

### Startup

At startup, send the CC15,16,17 and retrieve the existing settings.

Preload those settings into the controls before they become "active" otherwise
amongst other things the Clock will reset to 0 - Internal and everything goes
stupid.

### Docs

Sweep the manual for related material and consider putting it into the Info Text

By the same token, check all the CCs against reality - the manual is out of date
for some things

### Control interactions

Clock-in/Tempo - disable Tempo unless Clock-in is Internal

