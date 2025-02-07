# Game Design Document: Button Increaser

## 1. Overview

This document defines the simple game "Button Increaser".  
- Main resource: oTo (energy).  
- Player actions: click or tap a button to earn oTo.  
- Use oTo to buy upgrades that increase oTo gain.

## 2. Gameplay

- Core: Click or tap the main button to produce oTo.
- Upgrades: Spend oTo to:
    - Increase oTo per click/tap.
    - Produce oTo automatically over time.
    - Unlock new game features.
- Prestige: Option to reset progress for a permanent oTo boost.

## 3. Game Elements

- oTo Energy: The energy currency.
- Button: The element to click/tap that produces oTo.
- Upgrade Shop: Interface to purchase upgrades.
- Display: Shows current oTo amount and production rate.

## 4. Progression

- Spend oTo on upgrades.
- Upgrade costs grow exponentially.
- The system balances oTo production with cost increases.
- New Thresholds: When the player reaches key oTo levels (e.g., 1,000 oTo, 10,000 oTo), unlock special bonuses or new upgrade tiers.

## 6. Technical Considerations

- Platform: Mobile-friendly web browser.
- Engine/Library: JavaScript, CSS, JSON.
- Data Structures: Upgrade details stored in a JSON file; use simple structures (e.g., Maps) for fast lookups.
- Update Loop: Optimize calculations; refresh display only when needed.
- Event Handling: Use delegation for click/tap events.
- Mobile Optimization: Reduce DOM updates; use CSS transforms and requestAnimationFrame.
- Memory Management: Use object pooling to reduce garbage collection.
- Caching: Store frequently used DOM elements.
- Error Handling: Simplify error management to avoid slowdowns.
- Input Handling: Accept both mouse and touch signals; use passive listener and debouncing.
- Visuals: Render all graphics in basic classical ASCII art.
- Sound: Generate sound with an HTML oscillator tuned to a 432Hz scale.

## 7. Game Balance & Theory Considerations

- Scaling: Upgrade costs and rewards use exponential growth with oTo.
- Rewards: Upgrades must provide clear, incremental benefits.
- Decision Impact: Ensure clarity between quick tapping and sustained clicking.
- Refinement: Use simulations and player data to adjust parameters.
- Risk vs. Reward: Balance fast input rewards with long-term strategic benefits.
- Dynamic Difficulty: Gradually adjust the effect of tapping/clicking on oTo production.
- Threshold Bonuses: Integrate milestone rewards (e.g., at 1,000 oTo, 10,000 oTo) to provide extra incentives and mimic achievement events.

