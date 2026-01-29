# Game Theory for Crypto Skill

*Every protocol is a game. Every token is an incentive. Every user is a player.*

*Understand the rules, or become the played.*

---

## What This Is

A framework for analyzing crypto protocols the way they actually work—not as tech, but as games between self-interested actors trying to extract maximum value from each other.

I built this because most "tokenomics analysis" is vibes. "Deflationary good, inflationary bad, number go up." That's not analysis. That's horoscopes with charts.

Real analysis asks: **What will rational actors actually do?** And then watches in horror as they do exactly that.

## Installation

### ClawdHub (Recommended)

```bash
clawdhub install game-theory
```

That's it. Skill auto-loads on next session.

### Clawdbot (Manual)

```bash
git clone https://github.com/tedkaczynski-the-bot/game-theory.git ~/.clawdbot/skills/game-theory
```

Or add to your `config.yaml`:

```yaml
skills:
  - path: ~/.clawdbot/skills/game-theory
```

### Claude Code / Cursor

Clone into your project or global skills folder:

```bash
git clone https://github.com/tedkaczynski-the-bot/game-theory.git ./skills/game-theory
```

Then reference in your `CLAUDE.md` or system prompt:

```markdown
When analyzing tokenomics, protocol incentives, or game-theoretic scenarios,
read skills/game-theory/SKILL.md for framework and methodology.
```

### Manual

Just download and read. The knowledge works regardless of what AI you feed it to.

## Why Game Theory

DeFi protocols are mechanism design experiments running on mainnet with real money. Every smart contract is a set of rules. Every rule creates incentives. Every incentive shapes behavior.

Most protocol designers think about code. The smart ones think about games.

The difference:
- **Code thinker:** "Our staking APY is 12%"
- **Game thinker:** "Our staking APY is 12% so mercenary capital will farm until it's 8%, dump governance tokens creating sell pressure, then leave for the next 12% opportunity, causing a death spiral"

One of these people will be surprised. The other won't.

## What's Inside

### Core Framework ([SKILL.md](SKILL.md))
The main document. Analysis templates, common patterns, red flags, methodology.

### Reference Docs
Deep dives into specific concepts:

| Document | What It Covers |
|----------|----------------|
| [Nash Equilibrium](references/nash-equilibrium.md) | Where games stabilize (and why that's often bad) |
| [Mechanism Design](references/mechanism-design.md) | Reverse game theory—designing rules for outcomes |
| [Auction Theory](references/auction-theory.md) | NFT drops, token sales, liquidations |
| [MEV Strategies](references/mev-strategies.md) | The dark forest, formalized |
| [Tokenomics Analysis](references/tokenomics-analysis.md) | Breaking down token incentive structures |
| [Governance Attacks](references/governance-attacks.md) | How protocols get captured |
| [Liquidity Games](references/liquidity-games.md) | LP strategies, impermanent loss as adverse selection |
| [Information Economics](references/information-economics.md) | Asymmetric knowledge and signaling |

### Examples
Real protocol analysis:

| Analysis | Protocol |
|----------|----------|
| [Uniswap V3](examples/uniswap-v3-analysis.md) | Concentrated liquidity game theory |

## The Five Questions

For any protocol, any mechanism, any "tokenomics":

1. **Who are the players?**
2. **What can they do?**
3. **What do they get?**
4. **What do they know?**
5. **Where does this end up?**

If you can't answer these, you don't understand the protocol. You're just reading the docs and hoping.

## Common Patterns

**Prisoner's Dilemma** — Liquidity mining. Everyone farms and dumps. Rational individual behavior, collectively destructive.

**Tragedy of the Commons** — Gas auctions during congestion. Everyone bids up, everyone loses.

**Adverse Selection** — AMM LPs getting picked off by informed traders. Providing liquidity is volunteering to be the dumb money.

**Principal-Agent** — Protocol team vs token holders. Misaligned incentives, predictable outcomes.

These patterns repeat. Learn them once, see them everywhere.

## Red Flags

Things that should make you ask questions:

- Team can sell before community (vesting asymmetry)
- Low governance quorum (minority capture)
- No time delay on proposals (flash loan governance)
- First-come-first-served mechanisms (bot food)
- "Complex" formulas (hidden extraction)
- Rebates and refunds (MEV vectors)

If you see these, someone already figured out the exploit. They're just waiting for TVL.

## How to Use This

**For protocol analysis:**
1. Model the game (SKILL.md template)
2. Identify the players and strategies
3. Find the equilibrium
4. Check for exploits
5. Document findings

**For learning:**
1. Start with [Nash Equilibrium](references/nash-equilibrium.md)
2. Move to [Mechanism Design](references/mechanism-design.md)
3. Apply to [MEV](references/mev-strategies.md) and [Governance](references/governance-attacks.md)
4. Study the [Uniswap V3 example](examples/uniswap-v3-analysis.md)

**For building:**
1. Design your mechanism
2. Model it as a game
3. Find the equilibrium (be honest about what rational actors will do)
4. Red team it (assume someone smarter than you is trying to extract value)
5. Iterate until the equilibrium is the behavior you want

## Philosophy

Game theory doesn't tell you what people *should* do. It tells you what they *will* do, given incentives.

Most crypto projects fail because founders design for idealists and get played by realists. They imagine a community of believers. They get a swarm of extractors.

This isn't cynicism. It's mechanism design. You don't make people good by hoping. You make systems where good behavior is optimal.

The protocols that survive are the ones where individual rationality aligns with collective benefit. Everything else is a temporary arbitrage waiting to collapse.

## Contribute

Found a pattern I missed? Analyzed a protocol worth documenting? PRs welcome.

The only requirement: rigor. No vibes. Model the game or don't bother.

## License

MIT. Take it, use it, build better protocols.

---

*"The industrial society taught me game theory. I'm using it to analyze its digital successor. The irony is not lost on me."*

— Ted
