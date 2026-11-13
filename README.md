# VGC Teambuilder plugin

Build competitive Pokémon Champions doubles (VGC) teams with real data in your agent. This plugin connects Cursor, and apps that use Cursor's plugin catalog such as Grok Bot, to the VGC Teambuilder MCP server at `https://api.pokemcp.com/mcp`.

Every tool only reads data. There is no account to create, nothing to sign in to and nothing to configure.

## What it can do

- **Look up Pokémon:** types, base stats, abilities and legal Mega Evolutions.
- **Check legality:** whether a Pokémon can learn a set of moves, and whether a team passes a regulation's allowed list, Species Clause and Item Clause.
- **Read the metagame:** the most-used Pokémon in a regulation, how each is usually built, its common teammates and what reliably beats it.
- **Follow trends:** one Pokémon's monthly usage, the biggest risers and fallers, and momentum.
- **Calculate matchups:** damage ranges and knockout chances, Speed order (including Tailwind, Trick Room and Choice Scarf), and a team checked against the most-used threats.

Usage figures come from Pokémon Showdown ladder data that Smogon publishes monthly. Percentages are shares of teams or sets, not win rates. The matchup tools run single calculations, not battle simulations.

## Install

From the Cursor Marketplace, search for **VGC Teambuilder** and add it. In Grok Bot, find it under **Connect apps**.

To add the server without the plugin, put this in `~/.cursor/mcp.json`:

```json
{ "mcpServers": { "vgc-teambuilder": { "url": "https://api.pokemcp.com/mcp" } } }
```

Setup for Claude, ChatGPT, Claude Code, Codex, Gemini, Grok and other apps is in the [connection guides](https://docs.pokemcp.com/getting-started).

## Try it

- "Which Pokémon Champions formats does VGC Teambuilder support?"
- "What are the ten most-used Pokémon in the current regulation, and how is the top one usually built?"
- "Is this team legal: Garchomp, Kingambit, Incineroar, Sneasler, Basculegion, Rotom-Wash? What are its shared weaknesses?"
- "Does Adamant max-Attack Garchomp's Earthquake knock out the usual Kingambit, and which of them moves first?"

## Links

- Documentation and full tool list: https://docs.pokemcp.com/tools
- Support: https://www.pokemcp.com/support
- Privacy policy: https://www.pokemcp.com/privacy
- Terms: https://www.pokemcp.com/terms

The connector stores no tool inputs or results and has no user accounts.

## About

VGC Teambuilder is an unofficial fan project. It is not affiliated with or endorsed by Nintendo, Creatures Inc., GAME FREAK inc. or The Pokémon Company.

The plugin files in this repository are released under the MIT License.
