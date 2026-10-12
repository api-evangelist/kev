# Kev

Kev is an open-source (Apache-2.0) family of small decision models built on Qwen3.5/Qwen3.8 by Jared Palmer. The canonical home is https://github.com/jaredpalmer/kev. It is not a Cognition product.

## API

Kev runs as a self-hosted server (`python -m kev.serve`). The README documents these paths:

| Method | Path |
|---|---|
| POST | /v1/systemone |
| GET | /v1/models |
| POST | /v1/systemone/permute |
| POST | /v1/systemone/separate |

The question types are `noul`, `choice` and `score`. The README says (verbatim): "The API matches TypeSafe's System One, so you can point their Python SDK at your local server."

## Contract

The repository does not publish an OpenAPI, JSON Schema or protobuf contract. The full tree was searched on 2026-10-13. The API is documented only in prose in the README and implemented in `kev/api.py`. See `provenance/kev-contract-search.yml`.

## Links

- Demo: https://huggingface.co/spaces/jaredpalmer/kev
- Weights: https://huggingface.co/collections/jaredpalmer/kev-6aad9d0ea49f2589665e07cd
- Eval suites: https://huggingface.co/datasets/jaredpalmer/kev-suites
