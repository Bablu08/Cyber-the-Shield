# Buffer Overflow

> **Overview**: Buffer overflow basics and how they can be exploited.

## Explanation
When a program writes more data than a buffer can hold, leading to unexpected behavior.

**Example**:
Using Python to overflow:
```python
buffer = "A" * 5000

