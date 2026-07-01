# ICP Cloud Engines — plain-English guide

A short, honest guide to **ICP Sovereign Cloud Engines** — what you get **today** vs. what's still **roadmap** — from a developer coming off Rust backend canisters.

📄 **[Download the PDF →](./icp-cloud-engines-guide.pdf)**

> ⚠️ **Status honesty (mid-2026):** two headline features — **SEV confidentiality** and **owner-controlled upgrades** — are announced but **not live yet** (the OpenCloud node picker shows **0 SEV-SNP nodes** today; upgrades are still NNS-driven). Flagged 🔜 below. Don't build a launch on them yet.

The one idea: an engine is a **place**, not an app — essentially a **dedicated subnet you own** (min. 4 nodes), where you choose the hardware and geography. Your canisters run *on* it, unchanged.

## ✅ Real today
1. **Sovereignty** — choose the countries + operators; "EU-only" enforced by architecture.
2. **Single-tenant** — no noisy neighbors; the whole subnet's compute + storage is yours.
3. **No lock-in** — move between operators/countries within ICP, no rewrite, no downtime (`migrate-id` keeps the canister ID). Not an AWS→ICP importer.
4. **Hardware & size by choice** — pick node class (incl. cheaper, lower-spec); bigger = more storage/power per copy.
5. **Node count & predictable cost** — set replication (min. 4); flat per-node monthly, prepaid (80% to providers / 20% burned).

## 🔜 Announced — not live yet
6. **Encrypted computers (SEV-SNP)** — the intended privacy moat (operator can't read your data), but **0 SEV nodes available today**. Near-term roadmap, not a shippable guarantee.
7. **Owner-controlled upgrades** — today the **NNS** upgrades your engine like any subnet; owner control is planned later (consecutive-version catch-up caveat).
8. **GPU / on-chain AI** — CPU-only today; needs the "Gyrotron" milestone (announced, not shipped).

## ⛔ Doesn't change (same as any canister)
- Canister model · ~4 GiB heap / ~500 GiB stable per canister · instruction limits
- **vetKeys** for app-layer encryption — works on the public IC today, no engine needed
- **WASM only** — no Docker / Python / native; web2 stacks still get rebuilt as canisters

---

> Honest summary: today an engine = a dedicated subnet you own (geography, single-tenant, portability, hardware sizing, flat cost). The headline privacy (SEV) and owner-upgrades are *coming*, not here. It changes *where* your app runs and *who* runs it — never the app.

*Corrections welcome — the docs are still thin, and some of this is moving fast.*
