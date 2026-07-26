# hackindia-spark-11-hyderabad-telangana-south-central-region-hackflow
Hackathon team repository for HackFlow - [hackindia-team:hackindia-spark-11-hyderabad-telangana-south-central-region:hackflow]

Team HackFlow — Adaptive Concurrency-Aware Batcher for Cardano.

Submission lives entirely in the new ScrutinX/ folder (no other folders touched).

Reusable, adaptive batching infrastructure for Cardano's eUTXO model: it builds a contention graph of pending requests, solves Maximum Independent Set to pick the largest conflict-free batch, reads live congestion (EWMA of block fullness) to size the batch window, and settles the batch in one real Preprod transaction via an Aiken validator that enforces state-splitting to preserve concurrency for the next batch.

Demo video: https://drive.google.com/file/d/1QjhFBMEhw-VGWHVyT1qQqgPqNn5fgwBd/view?usp=sharing
Pitch deck: https://docs.google.com/presentation/d/1c0Wi2kVXDKgKpjQtwJc4StHBB5wTQmdr/edit?usp=sharing
Tech: Aiken (Plutus V3) · Lucid Evolution + Blockfrost (Preprod) · Next.js 14 + TypeScript + Tailwind + Zustand
Team members: Vikranth Sai, Jahwanth
