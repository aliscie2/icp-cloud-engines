# ICP Cloud Engines — plain-English guide

A short, plain-English guide to **ICP Sovereign Cloud Engines** — the 8 things an engine actually unlocks, ranked, from the perspective of a developer coming off Rust backend canisters.

📄 **[Download the PDF →](./icp-cloud-engines-guide.pdf)**

---

> The one idea: an engine is a **place**, not an app — a dedicated subnet you own. Your canisters run *on* it, unchanged. Same code, same limits; only the infrastructure changes.

## 🥇 The moat
1. 🔒 **Encrypted computers (SEV)** — no operator can read your data, and you can prove it (needs all nodes on SEV, which only "you pick the nodes" — an engine — can guarantee).
2. 🌍 **Sovereignty** — choose the countries + operators; "EU-only" enforced by architecture, not a contract clause.

## ⚙️ Operational wins
3. 🔓 **No lock-in** — move between operators/countries within ICP, no rewrite, no downtime (`migrate-id` keeps the canister ID). Not an AWS→ICP importer.
4. 🏠 **Single-tenant** — no noisy neighbors; the whole subnet's compute + storage is yours.

## 🔧 Control & knobs
5. 🎛️ **Upgrade control** — you approve when platform updates hit your engine.
6. 🧮 **Node count** — set replication; more nodes = more safety, not more capacity.
7. 💸 **Predictable cost** — flat per-node monthly, prepaid (80% to providers / 20% burned).
8. 📦 **Hardware grade** — pick node class (small → dense); bigger = more storage/power per copy.

## What does *not* change
- Canister model · ~4 GiB heap / ~500 GiB stable per canister · instruction limits
- vetKeys (works on the public IC too)
- **No GPU** — on-chain AI is roadmap ("Gyrotron"), not shipped
- WASM only — no Docker / Python / native

---

> One line: an engine changes *where your app runs, who runs it, who can see it, and how you pay* — never the app itself.

*Corrections welcome — the docs are still thin.*
