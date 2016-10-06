# redis-paulidecomposition
Lua script for Redis to apply pauli decomposition in PolSAR matrices.

## Requeriments

* Redis 3.2+ server running
* Lua 5.3+
* Three PolSAR matrices for each polarization (HH,HV,VV) stored in Redis Server

## Usage

`` redis-cli --eval paulidecomposition.lua <hash_mHH> <hash_mHV> <hash_mVV> ``

## Results

Three matrices are stored on the Redis: pauliReq, pauliGeq, pauliBeq.
