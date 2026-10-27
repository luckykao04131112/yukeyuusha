# Forestwatch: Thief Technology Campaign

This is an adaptation of the economic-defense loop described for Warcraft III's Xiao Tou Feng Kuang Ke Ji, not a complete or exact recreation of that map.

Reference: https://www.kkdzpt.com/fab/1037
Community reference: https://www.kkdzpt.com/fab/1037/637774fc15bcad5aa6cd6b89

Implemented:
- 60 waves; 20 leaked enemies lose the campaign. Every fifth wave has a boss.
- Roadside construction grid, not the former twelve fixed circular pads.
- Thieves earn gold on resolved hits, including killing hits; stale projectiles do not pay.
- Twelve upgrades in six thief ranks; shamans grant a non-stacking 30% attack-speed aura; frost casters slow enemies.
- Attack, haste and plunder technology, wood rewards and gold-to-wood purchases.
- Retained mobile hero, knight/assassin/smith classes, stat allocation and event-timed combat feedback.
- RTS-inspired bottom command panel and responsive mobile controls, using existing authorized-by-user RO sprites and custom scenery.

Not implemented from the original: exact map geometry and models, original unit values, carrier/fighter tech, Li Shu retirement economy, population upkeep, multiplayer and the complete original equipment tree.

Save key: forestwatch-thief-v1. Original forestwatch-hero-v2 and forestwatch-save-v1 remain untouched. The former playable build is backed up locally as forestwatch_hero_legacy.html. Saves are browser-local and do not sync between devices or origins.

Source: hero.html, hero.css, thief.css, hero-model.js, hero-game.js; shared atlas and sprite manifests unchanged.
Build: node work/package_forestwatch_hero.cjs
Verify: node work/verify_forestwatch_thief.cjs
Balance smoke test: node work/simulate_forestwatch_thief.cjs

The smoke test uses scripted purchases and a deterministic RNG. A successful 60-wave run is not a claim that all strategies or difficulties are balanced. Browser tests cover desktop/mobile viewport sizes, not performance on physical phones.
