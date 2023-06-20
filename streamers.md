![alt_text](https://i.imgur.com/e3HnZyI.png)

# Tournament Streamer Guidelines
This document is meant to give **Tournament Streamers** a few guidelines on streaming matches for the tournament.

First off, **thank you for volunteering to help with streaming matches!** As tournament streamers, we are the viewers' window to the action. Put simply, without you, this event would not be a success.

The following guidelines are intended to establish a set of standards designed to normalize all tournament-related streams. **These guidelines are required to be followed.** Feel free to ask the Tournament Director if you have any questions.


## Requirements
Every Tournament Streamer at minimum should:
```
1. Be able to run the game on MEDIUM to HIGH graphics settings (HIGH is preferred).
2. Have enough internet bandwidth and good enough hardware to stream at at least 1080p (1920x1080 or 1920x1200) resolution.
```


## I. Game Settings
Please set all KF2 Graphics options to the highest value(s) whenever possible to ensure the best quality image for the viewers. If nothing else, please make sure that at least Texture and Model Quality are set to **HIGH**.

Please turn off all in-game music. Some of the game's soundtrack is copyrighted material, which can lead to the stream's VOD being muted. Additionally, it can distract the viewers from being able to hear the commentators and the game itself.


## II. Game Modifications
Please remove/disable **any and all** visual, sound, or effect modifications (for example custom sounds) from your game before streaming matches.

The presence of these mods can detract from the production value / professionalism of the stream and in the case of some mods, can potentially hamper the viewer experience.


## III. Stream Resolution & Framerate
Please stream at *at least* **1080p** (`1920x1080` or `1920x1200`) resolution.

60 Frames per Second is strongly preferred, but not required.


## IV. Overlays, Stream Elements, & Audio
Please disable/hide any non-essential stream elements so that as much of the game is viewable as possible.
This includes:
```
1. Video cameras of any type
2. Subscriber / alert feeds
3. Any notifications and/or alerts (subscriber notifications, raids, donations, etc)
4. Any overlays / visual elements that are not designed to be a border of some sort
5. STEAM overlay notifications and sounds
```

Additionally, **please do not use copyrighted music** during the stream. This typically results in the stream's VOD being muted, which impacts the ability to rewatch the matches down the line.

A set of official tournament graphics, overlays, and transitions are available.

Please contact Tamari or ZeElmo for more information and directions on how to set everything up.

Here's an example of a good cast with great production quality and nice visuals:
https://youtu.be/M1EaEyw6i8I?t=1073

Some examples of casts from previous tournaments:
https://www.youtube.com/watch?v=YhYblPS91PA&list=PLuyPJLvrLKbQI5ywhaxACsHvw1tYZCo8U


## V. Server Specific Settings
By typing the `!settings` command into the **Chat Box** (T), the server's custom settings menu can be accessed.

Please make sure the following are in use for the stream:

**HUD**
```
Modern Scoreboard                      True
```
**HUD Elements: Main**
```
Global Large ZED Kill Ticker           True
ZED Time Counter                       True
```
**HUD Elements: World**
```
Player Info Type                       Name Only
```
**Gameplay: General**
```
Disable ZED Time Filter                False
Ignore Spectator Queue                 True
Cinematic Spectator Camera             True
```
**Miscellaneous**
```
Disable Cosmetics                      False
Spectator Camera Speed                 0.50
Enable Sobel Shader                    False
Clear Gore On Wave End                 False
```
**Colors**
```
Elite ZED Glow Color                   #8AD7DC
Fleshpound Glow Color                  #FAC819
Fleshpound Rage Glow Color             #FF4040
Speed Boost Status Color               #4444FF
Damage Boost Status Color              #FFFF44
Resistance Boost Status Color          #FF4444
```


## VI. Required Keybinds
### Camera Descent
An additional keybind is required to facilitate better control of the camera, namely, **allowing you to descend the camera without having to turn the view.** Currently, the JUMP key ascends the camera, but there is no default key for *descending* the camera.

To set the bind, simply enter one of the Match or Practice servers, and enter the following console command:

`setbind LeftControl "Button bDuck | Axis aUp Speed=-1.0 AbsoluteAxis=100"`


## VII. Camera Controls
This tournament uses a customized spectate system with enhanced features, enabling much more complex and precise control over the camera as well as providing additional information about the status of zeds, players, and the environment in order to communicate as much information to the viewer as possible.
```
1                           Jump to Player 1
2                           Jump to Player 2
3                           Jump to Player 3
4                           Jump to Player 4
5                           Jump to Player 5
6                           Jump to Player 6
7                           Jump to Next Boss
8                           Jump to Next Painted Target
9                           Jump to Objective Zone
LSHIFT (Hold)               Enable real-time movement during ZED Time (while in free camera)
LALT (Hold)                 Enable mouse cursor (see below for more info)
LALT + LeftMouseButton      Jump to Target (when hovering over ZED or player)
LALT + LeftMouseButton      Jump to Player (when hovering over a player's Status Pane)
LALT + LeftMouseButton      Jump to ZED (when hovering over ZED health bar)
LALT + RightMouseButton     Paint ZED
```

## VIII. Conduct
Please keep it professional. Your behavior directly reflects on the tournament organization as a whole.

In the event that a Tournament Streamer also functions as a **Commentator**, they should be as professional as possible and avoid using excessive foul language and/or behaving in a crude or immature manner.


## IX. Ownership
Tamari's KF2 Tournaments does not own the content you produce related to our tournament(s).

However, by agreeing to stream the matches, you consent to us downloading your VODs and uploading them to the official tournament channels (YouTube, etc).
