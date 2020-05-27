# rpi_wordclock_for_homeassistant
Makes a rpi_wordclock available to home assistant as light 

If you build a [rpi_wordclock](https://github.com/bk1285/rpi_wordclock), you can make use of this repository to integrate it to your homeassistant framework as follows:

* Go to the config-directory of your home assistant instance:
  
  E.g. ```cd ~/.homeassistant/custom_components/```
  
 * Place the rpi_wordclock folder from this repository inside this folder.
 
 * Now you're ready to add a rpi_wordclock with its specific IP address to your configuration.yaml

    ```
    light:
    - platform: rpi_wordclock
      host: 192.168.YOUR.IP
      name: "Wordclock"
    ```

 * Finish by restarting home assistant.
