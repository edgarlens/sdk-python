# Edgar Lens Python SDK

Official Python SDK for the Edgar Lens API.

## Features
- Sync & async clients
- Typed models (pydantic)
- Pagination & retries
- Great for notebooks and ETL

## Installation
```bash
pip install edgarlens
```

## Quick Start
```python
from edgarlens import EdgarLens

client = EdgarLens(api_key="YOUR_API_KEY")
diffs = client.diffs.get(ticker="AAPL")
print(diffs)
```

## Async Example
```python
import asyncio
from edgarlens import AsyncEdgarLens

async def main():
    client = AsyncEdgarLens(api_key="YOUR_API_KEY")
    diffs = await client.diffs.get(ticker="AAPL")
    print(diffs)

asyncio.run(main())
```

## Versioning
Matches the API's semantic versioning.

## License
MIT — see [LICENSE](LICENSE).
