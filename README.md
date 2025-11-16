# Long-Form Story Generator via AI and Editing Automation
### Introduction
This project generates long form story videos through an input script. Through editing automation as well as text to speech and text to image one can obtain results like the following:

**Comic Style** (Screenshot)
![Example 1](https://github.com/jimmyjjz/lfs-vid-gen/blob/main/example_image_1.png)

**Youtube Roblox Story Style** (Screenshot)
![Example 2](https://github.com/jimmyjjz/lfs-vid-gen/blob/main/example_image_2.png)

Example videos: https://www.youtube.com/@Robloxuha.

When it comes to the script one can generate it through LLM(s) or write it manually(For formatting specifications please read prompt outputted via [main.py](https://github.com/jimmyjjz/lfs-vid-gen/blob/main/story-video-generator/main.py)).

Customizability:
- Animations and motion can be altered(If you understand python and want to learn more visit [animateable.py](https://github.com/jimmyjjz/lfs-vid-gen/blob/main/story-video-generator/animateable.py)).
- Setting max vram usage.
- Switching AI models for different tasks.
- Visual images can be any images you want.
- Background can be any video you want.
- Toggleable intermission/title segment.
- Dimensions of the outputted video.
- Generated any number of videos you want.
- Any intro/watermark(animated, video, image, etc) you want.
- And more...

### Setup
1. Enter a python environment.
2. Make sure you are using python 3.11+ interpreter.
3. Install dependencies
```
pip install tortoise_tts==3.0.0 moviepy==2.1.0 diffuser==0.32.1 pydirectinput==1.0.4 faster_whisper==1.1.0
```
4. (Reccomended) Download the version of pytorch that fits your hardware. Visit https://pytorch.org/get-started/locally/ for details.

In the scenario that you are not able or refuse to then
```
pip install pytorch==2.5.1
```

### Usage
1. Setup settings, proceed through [settings.json](https://github.com/jimmyjjz/lfs-vid-gen/blob/main/story-video-generator/settings.json)
2. Get a adequately sized mp4(s), name them bgvid# #=1,2,3..., and then throw them into [story-video-generator folder](https://github.com/jimmyjjz/lfs-vid-gen/tree/main/story-video-generator)
3. Obtain/Create a formatted script and copy-paste it into [script.txt](https://github.com/jimmyjjz/lfs-vid-gen/blob/main/story-video-generator/script.txt).
4. (Reccomended) Run [script_check.py](https://github.com/jimmyjjz/lfs-vid-gen/blob/main/story-video-generator/script_check.py) and if necessary fix up your script.
5. Free up enough vram(Expect ~4-5gb for ~15min video on highest cost mode)
6. Run [main.py](https://github.com/jimmyjjz/lfs-vid-gen/blob/main/story-video-generator/main.py)
