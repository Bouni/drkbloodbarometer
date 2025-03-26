g DRK-Blood-Barometer

A python library that extract the current levels of donated blood from the website of a given states DRK (German red cross) website.

## Installation

```sh
pip install drk-blood-barometer
```

## Usage

```python

from drkbloodbarometer import DRKBloodBarometer

bb = DRKBloodBarometer("Baden-Würtemberg")

print(bb.bloodlevels)
print(bb.lastChange)
```

The result looks like this

```
{
    "A+": {"level": 29.4, "warning": False, "rating": "Kritisch"},
    "B+": {"level": 37.2, "warning": False, "rating": "Kritisch"},
    "AB+": {"level": 38.4, "warning": False, "rating": "Kritisch"},
    "0+": {"level": 16.2, "warning": False, "rating": "Bedrohlich"},
    "A-": {"level": 16.2, "warning": False, "rating": "Bedrohlich"},
    "B-": {"level": 29.4, "warning": False, "rating": "Kritisch"},
    "AB-": {"level": 36.0, "warning": False, "rating": "Kritisch"},
    "0-": {"level": 15.6, "warning": True, "rating": "Kritisch"},
}
2025-03-20 00:00:00
```

## Disclaimer

The author is not in any way affiliated with DRK. This library is neither offered nor supported by DRK. The authors do not take any liability for possible damages.
