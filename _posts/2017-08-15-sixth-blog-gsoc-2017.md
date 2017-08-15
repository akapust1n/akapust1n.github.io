Hi, this post is general information about telemetry in Krita. I want to clarify some points.

Soon we will launch a preliminary testing of my [branch](https://github.com/KDE/krita/tree/akapustin/T6102-telemetry). 
In case of successful testing, it will go into one of the closest releases of Krita (not  3.2).
Krita must follow the policy of the KDE on [information gathering](https://mail.kde.org/pipermail/kde-community/2017q3/003806.html).
What information do we want to collect?
  * General information about your system: version of Os, number of processor cores and etc
  * General information about what you are pressing in Krita, what brushes you use, whether you often use gradients and etc.
  * General information about what images you draw: image resolution, weight, number of layers and etc.
  * Information on the incorrect completion of the program

The collected statistics will help us make Kreta better. It is absolutely anonymous.
We do not transmit data that could be used to identify a specific user. In 
particular:
  * we will not use any unique device, installation or user id
  * data is stripped of any unnecessary detail and downsampled appropriately 
before sharing to avoid fingerprinting.

At any time you can turn off sending statistics.

