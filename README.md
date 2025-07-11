# ErcNftIndexer

## Description



## Features

- Indexes ERC-721 and ERC-1155 token metadata, including images and descriptions, from IPFS and Arweave.
- Stores indexed NFT data in a PostgreSQL database optimized for fast querying and filtering.
- Exposes a GraphQL API for efficient and flexible retrieval of NFT data based on custom criteria.
- Subscribes to blockchain events using WebSockets to provide real-time updates on NFT transfers and mints.
- Implements a caching layer using Redis to minimize database load and improve API response times.
- Supports configurable backfilling of historical NFT data from specified block ranges.
- Monitors and logs indexing performance metrics using Prometheus and Grafana for proactive issue detection.
- Integrates with OpenSea's API to enrich NFT data with marketplace information, such as floor price and trading volume.
## Installation

```bash
npm install ercnftindexer
```

## Usage

```typescript
import { ErcNftIndexer } from 'ercnftindexer';

const app = new ErcNftIndexer({ verbose: true });
app.execute();
```

## Contributing

We welcome contributions! Here's how to get started:

1. Fork this repository
2. Create a new branch for your feature (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add some awesome feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.
