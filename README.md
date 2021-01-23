# HalfHeardVoicesLightShow

Uses Chauvet ShowXpress and Ableton Live to route Ableton lightshow Midi synced via backtracks Chalet ShowXpress, which routes the midi to the DMX interface which then controls our lights. 

Place under ~/TheLightingController/Lightshows (this is separate from the install path). 


To hook up ShowExpress to Ableton Live via a virtual midi interface see here: https://www.youtube.com/watch?v=59IVJgNoDME 

### Steps:
- Open the Audio Midi Setup app on Mac 
- In Audio Devices: Window > Midi Studio > IAC Driver > Add port called "From Ableton" or similar descriptive name, and click "Device is Online".
- In Ableton, on the midi track configure the output of the track to use the IAC Driver (From Ableton) or whatever you named the port. Set Track ON for the output. After editing preferences ensure that you actually select the IAC Driver and it is not grayed out. Regular light midi on channel 1, pixels on channel 2. 
- In ShowExpress, Go to Preferences > Midi. REMOVE the default track for Midi In. Add the IAC Driver From Ableton on channel 1. Device Type is Default. Hit Apply. 
-Now when you run Ableton, you should see the buttons being controlled in ShowExpress by the midi tracks. You may need to ensure the XLR cable button/midi button is enabled on the top right to enable the live mode.  
