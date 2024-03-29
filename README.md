
## Status

This project is here for historical purposes. It no longer builds on modern linux distrubutions and only worked on KDE3.x. Anyone is welcome to update the build files to something more modern and to update it to a modern version of QT and KDE.

## Documentation

       This plugin contains macros that can be used in a configuration file that 
       facilitates contolling of KDE applications. This plugin package actually 
       contains the following plugins:

       amarok_plugin
       juk_plugin
       kscd_plugin
       kdesktop_plugin
       kmail_plugin
       kmix_plugin
       konqueror_plugin

amarok_plugin
       The Amarok plugin supports 13 macros to control the behaviour of the 
       amarok application. These macros are:

       AMAROK_PLAY, AMAROK_PAUSE, AMAROK_STOP, AMAROK_PLAYPAUSE, AMAROK_BACK, 
       AMAROK_FORWARD, AMAROK_SEEK, AMAROK_ADDMEDIA, AMAROK_VOLUMEUP, 
       AMAROK_VOLUMEDOWN, AMAROK_VOLUMEMUTE, AMAROK_TOGGLEPLAYLIST, 
       AMAROK_ENABLERANDOM

kscd_plugin
       The Kscd plugin supports 12 macros to control the behaviour of the kscd 
       application. These macros are:

       KSCD_PLAY, KSCD_PAUSE, KSCD_STOP, KSCD_PREVIOUS, KSCD_NEXT, KSCD_EJECT, 
       KSCD_TOGGLE_LOOP, KSCD_TOGGLE_SHUFFLE, KSCD_TOGGLE_TIME_DISPLAY, 
       KSCD_CURRENT_TRACK, KSCD_CURRENT_ALBUM, KSCD_CURRENT_ARTIST

juk_plugin

       The  Juk  plugin  supports 13 Macros to control the behavior of the Juk
       application. These macros are:

       JUK_PLAY, JUK_PAUSE, JUK_STOP,  JUK_PLAYPAUSE,  JUK_BACK,  JUK_FORWARD,
       JUK_SEEKBACK,  JUK_SEEKFORWARD,  JUK_VOLUMEUP, JUK_VOLUMEDOWN, JUK_VOL-
       UMEMUTE, JUK_STARTPLAYINGPLAYLIST, JUK_OPENFILE

kscd_plugin
       The Kscd plugin supports 12 macros to control the behaviour of the kscd 
       application. These macros are:

       KSCD_PLAY, KSCD_PAUSE, KSCD_STOP, KSCD_PREVIOUS, KSCD_NEXT, KSCD_EJECT, 
       KSCD_TOGGLE_LOOP, KSCD_TOGGLE_SHUFFLE, KSCD_TOGGLE_TIME_DISPLAY, 
       KSCD_CURRENT_TRACK, KSCD_CURRENT_ALBUM, KSCD_CURRENT_ARTIST

kdesktop_plugin
       The kdesktop plugin supports 5  macros.  These  are:  KDE_LOCK_DESKTOP,
       KMENU,   KDESKTOP_NEXT,   KDESKTOP_PREVIOUS,  KDESKTOP_EXECUTE.  KDESK-
       TOP_EXECUTE will open the command line execution dialog box.


kmail_plugin
       The KMail plugin supports only one Macro: KMAIL_COMPOSE.  However  this
       macro can take up to 5 arguments:

       KMAIL_COMPOSE(from,to,cc,subject,attachment) The attachment is in form
       of a URL.


kmix_plugin
       The   kmix   plugin  supports  three  macros.  These  are:  KMIX_VOLUP,
       KMIX_VOLDOWN, KMIX_MUTE. These macros follow the EAK_ style  macros  in
       that they support options.

       KMIX_MUTE
              This  is  the default form of the macro. If used in this form it
              will mute the first mixer to a volume of 0.

       KMIX_MUTE(X)
              Here X is a kmix mixer. You can get a list of  mixers  that  are
              supported by running: dcop kmix

       KMIX_MUTE(device,device2,device3,...)
              Here  deviceX  is a string name of a mixer device (e.g. "Mixer0"
              to mute.) This allows you to mute more than one mixer at a time.

       For  the  KMIX_VOLUP  and  KMIX_VOLDOWN macros. Each have the following
       forms.

       KMIX_VOLUP or KMIX_VOLDOWN
              Increment or decrement the default mixer by an increment of 5.

       KMIX_VOLUP(X) or KMIX_VOLDOWN(X)
              Increment or decrement the default kmix mixer by a value of X.

       KMIX_VOLUP(X,device,X2,device2,X3,device3,...) or
       KMIX_VOLDOWN(X,device,X2,device2,X3,device3,...)
              X is the volume to adjust the following device by.


konqueror_plugin
       The  konqueror  plugin supports just one macro KONQUEROR. However, this
       macro can take arguments to control  an  instance  of  konqueror.   You
       should note that this will control the first instance of konqueror that
       it can find. It cannot as of yet target the  active  instance  of  kon-
       queror.  Until  dcop/kwin/konqueror  supports  a  way to get the active
       instance of konqueror, this is nothing that can be done about this.

       By itself the KONQUEROR macro will start an instance  of  konqueror  if
       there is not one already running.

       Here are the following arguments that are possible with this macro.

       back
       forward
       home
       stop
       refresh or reload
       newtab
       bookmark
