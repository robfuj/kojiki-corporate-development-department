# Bots of Corporate Development  (docx S5 candidate menu)

These are the **Major sub-functions** of Corporate Development from the spec. Each is a bot — a
child decision system that can be instantiated to do the actual work.

## Install flow (matches the Orientation Protocol)
1. **Orient** — the agent runs the Kojiki Orientation Protocol (name / industry /
   jurisdiction / siblings).
2. **Research** — the agent researches the field and decides which sub-functions this
   specific org needs.
3. **Install** — instantiate only the chosen bots:
   ```bash
   cd bots
   python3 install_bots.py brand growth performance-marketing
   ```
   (use the slugs listed below; omit args to install all). Each installed bot becomes a
   full decision system under `bots/<slug>/` with README + AGENT.md + schemas + a stub
   decision record, and registers under this department's group_id for handoffs.

Total candidates: 7.

- `m-a` — **M&A**  ·  titles: Chief Corporate Development Officer, VP Corporate Development, Corp Dev Director, M&A Director, Investment Manager, Integration Director
- `investments` — **Investments**  ·  titles: Chief Corporate Development Officer, VP Corporate Development, Corp Dev Director, M&A Director, Investment Manager, Integration Director
- `corporate-ventures` — **Corporate Ventures**  ·  titles: Chief Corporate Development Officer, VP Corporate Development, Corp Dev Director, M&A Director, Investment Manager, Integration Director
- `strategic-transactions` — **Strategic Transactions**  ·  titles: Chief Corporate Development Officer, VP Corporate Development, Corp Dev Director, M&A Director, Investment Manager, Integration Director
- `target-intelligence` — **Target Intelligence**  ·  titles: Chief Corporate Development Officer, VP Corporate Development, Corp Dev Director, M&A Director, Investment Manager, Integration Director
- `due-diligence` — **Due Diligence**  ·  titles: Chief Corporate Development Officer, VP Corporate Development, Corp Dev Director, M&A Director, Investment Manager, Integration Director
- `integration` — **Integration**  ·  titles: Chief Corporate Development Officer, VP Corporate Development, Corp Dev Director, M&A Director, Investment Manager, Integration Director
