sudo apt-get update && sudo apt-get install -y libdbus-1{,-dev}
pip install omxplayer-wrapper

#!/usr/bin/env python3

from omxplayer.player import OMXPlayer
from pathlib import Path
from time import sleep

VIDEO_PATH = Path("../tests/media/test_media_1.mp4")

player = OMXPlayer(VIDEO_PATH)

sleep(5)

player.quit()
