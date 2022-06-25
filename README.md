Works only if music requests is free.

# Easy streamdj.app
Created for easyer send/skip tracks in streamdj.app.  
proxy list for skip tracks from [here](https://github.com/TheSpeedX/PROXY-List)

## Examples

send one track:
```bash
python -m easy_streamdj some_channel --video "https://www.youtube.com/watch?v=dQw4w9WgXcQ"

```

send playlist of tracks:
```bash
python -m easy_streamdj some_channel --playlist "https://www.youtube.com/playlist?list=PL2aMEXnwcG3nqpr49qfCJ5vLTuxImPdme"
```

send playlist first playlist finded on youtube:
```bash
python -m easy_streamdj some_channel --playlistserch "good music"
```

skip current track:
```bash
python -m easy_streamdj some_channel --skip
```

run easy streamdj over tor:
```bash
sudo systemctl start tor  # start tor service if it is not started already
torify python -m easy_streamdj some_channel -P "bad music" --delay 12 --author "anonymous"
```

get some help:
```bash
python -m easy_streamdj
```

## Installation
Install [python3.10+](https://www.python.org/downloads/)
```bash
git clone https://github.com/e6000000000/easy_streamdj.git
cd easy_streamdj
pip install poetry
poetry build
pip install dist/*.whl
```
