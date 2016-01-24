# makamusicbrainz
Packages to fetch metadata related to the makam music recordings and works from MusicBrainz

Usage
============
```python
from makammusicbrainz.audiometadata import getAudioMetadata
audio_meta = getAudioMetadata(mp3file, getWorkAttributes=True)

from makammusicbrainz.workmetadata import getWorkMetadata
work_meta = getWorkMetadata(work_mbid)
```

Please refer to [demo.ipynb](https://github.com/sertansenturk/makammusicbrainz/blob/master/demo.ipynb) for an interactive demo.

Installation
============

If you want to install makammetadata, it is recommended to install makammetadata and dependencies into a virtualenv. In the terminal, do the following:

    virtualenv env
    source env/bin/activate
    python setup.py install

If you want to be able to edit files and have the changes be reflected, then
install compmusic like this instead

    pip install -e .

Now you can install the rest of the dependencies:

    pip install -r requirements

Authors
-------
Sertan Senturk
contact@sertansenturk.com

Acknowledgements
------
We would like to thank Dr. Robert Grafias for allowing us to use [his makam music collection](https://eee.uci.edu/programs/rgarfias/films.html) in our research (in this repository the recording with MBID: [635530df-8e13-4587-a94d-32f3c1643ca6](http://musicbrainz.org/recording/635530df-8e13-4587-a94d-32f3c1643ca6)).
