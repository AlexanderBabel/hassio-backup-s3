# HomePod Connect

This addons allows to use OwnTone and Spotify Connect with librespot-java on Home Assistant OS.


## Configuration

(You can use the VSCode add-on to customize the configuration.)

You can configure OwnTone through its configuration file. It can be found at `/config/owntone/owntone.conf`.

Librespot-java is configurable through its configuration file at `/config/owntone/librespot-java.toml`

The configuration page allows you to enable/disable the Airplay instances, name them, change the tcp/udp port if needed, and choose from two logging levels. The Airplay instances are also configurable through thier configuration files at `/config/owntone/shairport-sync-pipe.conf` and `/config/owntone/shairport-sync-audio.conf`.

Also on the configuration page, the [librespot-java](https://github.com/librespot-org/librespot-java) cache can be enabled/disabled and the Home Assistant audio device can be chosen.

Please note, the Airplay instance that will pipe audio and metadata to Owntone for whole house audio will pause play on librespot-java when a device connects to it to prevent overlapping garbled sound.  When the device disconnects form the Airplay instance, it may take a few seconds for the pipe to clear and librespot-java can provide clear audio.

After adjusting something, please restart the add-on.


## Access OwnTone

You can access OwnTone through `[Home Assistant IP]:3689`


## OwnTone Credentials

Username: `admin`

Password: `owntoneadmin8765`
