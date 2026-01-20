#System Architecture


## Architecture Overview

The system follows a layered architecture that separates medical record management
from blockchain integrity verification.

### Layers
1. Presentation Layer (CLI / REST API)
2. Medical Record Layer
3. Blockchain Layer
4. Storage Layer

### Data Flow
1. A medical record is created by an authorized user
2. The record is serialized and hashed using SHA-256
3. The record i stored off-chain
4. The hash and metadata are stored in a blockchain block
5. Blockchain validation detects any tampering
