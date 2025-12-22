# react-zephyr

A minimal event-driven framework for React state management.

### Installation

```bash
pip install react-zephyr
```

### Usage

Define an event handler and register it with the state controller:

```python
from reactzephyr import Zephyr

app = Zephyr()

@app.on("update_count")
def handle_count(state, payload):
    state["count"] += payload

app.emit("update_count", 1)
```

### License

MIT License

