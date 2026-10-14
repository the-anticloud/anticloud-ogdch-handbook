# Build and Test

**Project:** `OGDCH_HANDBOOK`
**Upstream:** https://github.com/opendata-swiss/ogdch_handbook
**License:** MIT

## Quick Start

```bash
git clone https://github.com/opendata-swiss/ogdch_handbook
cd ogdch_handbook
pip install -r requirements-anticloud.txt
python anticloud_main.py --offline --pax-local
```

## Anticloud Improvements Applied

1. PAX L5 Narrow L2 General 27B local document processing — air-gapped sovereign deployment
2. AIOSS tamper-evident audit trail for all citizen record modifications
3. AES-256 encryption aligned with FIPS 140-2 for all stored data
4. Single-binary deployment on sovereign government infrastructure
5. Zero third-party cloud: no data leaves government-controlled servers
6. Role-based access control with cryptographic audit log of all access
7. Offline NLP pipeline for form processing and classification
8. Open-source supply chain: all dependencies pinned, audited, MIT/Apache 2.0

## Benchmark Targets

| Metric | Target |
| --- | --- |
| Latency | Primary inference task: <5s on CPU, <1s on GPU |
| Throughput | Batch processing: >100 items/hour on single CPU server |
| Memory | <8GB RAM for standard deployment |
| Accuracy | Task-specific accuracy within 5% of cloud-API baseline |

## Build Status

Not yet measured. Run verified build and record actual figures above.
