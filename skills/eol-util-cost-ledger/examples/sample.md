# Worked example: Cost Ledger

**Fictional product, illustrative figures.** Continues from the Zombie ID Card example.

| | |
|---|---|
| **Product** | Classic Reports |
| **Zombie ID verdict** | Zombie |
| **Period** | Annual |
| **Prepared by** | The product manager covering Classic Reports |

## What it earns (above the line)

| Line | Amount or range | Label | Source |
|---|---|---|---|
| Revenue and renewals | $1.1M to $1.2M, down three years running | measured | Finance renewal report *(illustrative)* |
| Strategic value | 12 multi-year contracts name Classic Reports; two are reference accounts for Insights | measured | Contract list |

## What it eats (below the line)

| Line | People | Amount or range | Label | Source |
|---|---|---|---|---|
| Support load | About 2 support agents | $180K to $220K | estimated | Ticket share times team cost; tickets per customer up three years |
| Maintenance effort | About a third of one squad (3 engineers) | $450K to $550K | estimated | Squad lead's sprint history |
| Compliance and security exposure | Part of one security review cycle | $40K to $80K | estimated | Last audit's findings on the old engine |
| Technical debt it holds in place | Blocks retiring the old reporting engine | Engine vendor support ends next year; extended support quoted at $150K | measured | Vendor quote |
| Infrastructure and licenses | | $60K | measured | Hosting and engine license invoices |

## What it forgoes (off the books)

| Line | What, specifically |
|---|---|
| The next bet this capacity would fund | The fuel-tax module in Insights, then live alerts for fleet managers |
| Roadmap room it occupies | One squad's maintenance slot every sprint; one quarterly planning fight |

## The net

**Earns minus eats:** roughly break-even this year (between a $60K surplus and a $160K loss), and worse next year once extended engine support is due.

**Plus what it forgoes:** the fuel-tax module that would let the 12 contracted customers move to Insights, and the alerts feature after it.

## The waterline sentence

What it earns above the line: about $1.1M from a shrinking base. What it eats below: two support agents, a third of a squad, an engine that loses support next year, and the module that would let its customers move on.

## Questions for finance

| # | Unknown | Could it change the answer? |
|---|---|---|
| 1 | Allocated shared costs (sales, account management) | Yes: would push it clearly to a loss |
| 2 | Renewal risk on the 12 contracts if notice is given | Yes: sizes the migration discount |

## Next step

- Run `eol-step2-revive-or-replace` with this ledger and the Zombie ID Card.
- After the exit, run `eol-step4-free-the-living` to move the squad and support capacity it frees.
