# How to use JSON files

### How to use print a dictionary nicely formatted
```python
import json

data = {'name': 'RT1',
        'ip': '192.168.1.25',
        'platform': 'ios'}

print(json.dumps(data, indent=4))
```

### Load a json file
```python
import json

with open('myjsonfile.json', 'r') as f:
    data = json.load(f)

print(json.dumps(data, indent=4))
```

### Saving data as a JSON file.
```python
import json

data = {'name': 'RT1',
        'ip': '192.168.1.25',
        'platform': 'ios'}

with open('myjsonfile.json', 'w') as f:
    json.dump(data, f)
```
