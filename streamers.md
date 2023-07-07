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

## Videos on Demand (VODs)
Please ensure that your Twitch channel is set to archive Past Broadcasts. You can find information on how to achieve this here: https://help.twitch.tv/s/article/video-on-demand?language=en_US

Enabling stream archiving ensures that the broadcasts can be downloaded and uploaded onto the official tournament YouTube channel.

## Streamer Content
We'll be using a customized set of OBS scenes and Stinger Transitions for this tournament. Please see the dedicated #streamers channel in the tournament Discord for a link to the files as well as a guide explaining how to set everything up.

## Procedure
The general procedure of a stream goes as follows:

### Starting the Stream
1.  Plan to be early. It's best to start the stream about **15-20 minutes** before the match's start time to avoid delays (ie: if a match is scheduled for 2 PM, start the stream at 1:45 PM at the latest). This gives plenty of time for the casters to introduce the match, give a roster rundown, talk about the map, explain the scoring system, and so on, all while letting the match start on time.
2.  Mute your Microphone and Desktop Audio in OBS so that you can freely coordinate with the casters without the streams viewers being able to hear.
3.  Allow the timer on the Starting Soon Scene to reach zero, or at least 5 minutes remaining. This gives the audience a chance to join the stream.
4.  After the timer expires, and when the casters are ready, swap to the in-game "Main" scene. Then, give the commentators a countdown before you unmute your Desktop Audio in OBS. This allows them to know when they are on the air and when it's appropriate to start speaking.
5.  Upon reaching the match's designed Start Time, double-check that the commentators are ready and let the team that is playing know that you are ready to go. **Note that in the event that the players are ready before the match's scheduled Start Time, you are NOT required to end the introduction segment early.**

### War Rooms
War Rooms refer to the streaming/casting staff dropping into the team's voice chat to listen in on their comms, and they are a great way of giving the viewers a more personalized account of the action. It is the attending casters'/commentators' responsibility to determine when to enter the team's War Room.

As the streamer, you should ensure the following:
1.  Your microphone is muted and/or set to Push to Talk.
2.  You have switched to the proper **Discord Voice Chat Overlay** so that the viewers can see who is speaking in the War Room. See the dedicated #streamers channel in the tournament Discord, where a guide can be found on how to properly achieve this.

**You should avoid minimizing your game to enter the War Room.** This will cause the game audio to cut out, which can be jarring for the viewers. To combat this, the Lead Commentator will manually move you in and out of the team's War Room.

### Replays
Throughout the match, highlights can be shown in the form of **Replays.** Replays allow us to save the coolest moments of a match and show them to the viewers to generate some hype and highlight a specific moment. See the dedicated #streamers channel in the tournament Discord, where a guide can be found on how to properly set up Replays.

In general, the best times to save a replay are:
1.  During "clutch" scenarios where one player makes a game-changing play
2.  During the Boss Wave
3.  During situations where multiple players die from a Zed attack, environmental hazard, or otherwise
4.  During a moment of high-performance from a specific player, such as a player achieving multiple Large Zed takedowns in a short time, an impressive Zed Time Extension combination from a Commando, and so on

The best times to **show** the replay to the viewers are:
1.  During the Trader period
2.  During the Postgame Interview session

Refrain from showing too many replays during the match, as they can take away from the viewer's ability to see what's going on. This is especially true during the Trader period, where some important/game-changing strategies might come to fruition from the team. In general, a fair amount of replays to show per match is around **5.**

### Postgame Interviews
Typically, after the match concludes, the commentators will pull one or two of the players from the team into the caster war room to conduct **Postgame Interviews**. During this time, you are welcome to unmute your microphone and ask questions to the players if desired. Otherwise, there is not much to be done. If desired, you are welcome to fly the camera around the map and give the viewers some nice scenery while they listen to the interview.

### Ending the Stream
When it's time to end the stream:
1.  Mute your Desktop Audio in OBS
2.  Switch to the "Stream Ending" scene
3.  After a few minutes, end the stream

## I. Game Settings
Please ensure the following game settings:
- All Graphics options set to the highest value(s) whenever possible. If nothing else, please make sure that at least Texture and Model Quality are set to **HIGH**.
- Game Music volume set to 0%. Some of the game's soundtrack is copyrighted material, which can lead to the stream's VOD being muted. Additionally, it can distract the viewers from being able to hear the commentators and the game itself.

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

A set of official tournament graphics, overlays, and transitions are available. See [above](https://github.com/tamari92/kf2-tournament/blob/summer23/streamers.md#streamer-content) for more information.

Please contact Tamari or ZeElmo for more information and directions on how to set everything up.

Here's an example of a good cast with great production quality and nice visuals:
https://youtu.be/M1EaEyw6i8I?t=1073

Some examples of casts from previous tournaments:
https://www.youtube.com/watch?v=YhYblPS91PA&list=PLuyPJLvrLKbQI5ywhaxACsHvw1tYZCo8U


## V. Server Specific Settings
There are some server-specific settings that you'll need to set for this tournament. To access them, join any of Tamari's servers and type the `!settings` command into the **Chat Box** (T).

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

To set the bind, simply enter any of Tamari's servers, and enter the following console command:

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
9                           Jump to active Objective Zone
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
