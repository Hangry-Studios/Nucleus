# Nucleus 🔵

A dopamine-optimized fake casino — TikTok-style.

Nucleus is a single-file web app where each casino game fills the entire screen. Lose (or win) and the next game snaps into view — exactly like scrolling a feed. No real money, no downloads, no backend. Just a pure dopamine loop in 77 KB of HTML.

## Games
GameMechanic🎰SlotsWeighted reel symbols, near-miss injection, auto-spin toggle🃏BlackjackFull rules — hit, stand, double down, dealer AI🎡Spin WheelCanvas-animated wheel, 12 segments, physics easing💣Mines5×5 grid, growing multiplier, cash out anytime🎲Dice DuelRoll against the house, animated dice🃟Hi-LoGuess higher/lower, chain correct guesses to build multiplier🔵PlinkoPhysics-simulated ball drops through 8 rows of pins
Games are shuffled into a random order every session. The feed is infinite — when you reach the end of a round, a new shuffled round is appended automatically.

## Features
Coin system

Start with 1 000 🪙
Daily login bonus of +200 🪙
4 bet sizes: 10 / 50 / 100 / 500
Broke screen with a 5-minute timer to claim 200 free coins
All balances persist in localStorage

## Addiction mechanics

Auto-scroll to the next game 1.5 s after a loss
Near-miss animations on slots (two matching reels)
Win streak multiplier — 3+ wins in a row = 2× payout
Streak badge shown on consecutive wins

## Effects

Confetti bursts, coin showers, particle explosions on wins
Full-screen radial flash (green on win, red on loss)
Screen shake on loss
Glassmorphism Big Win overlay with staggered animations
Floating +XP / amount text anchored to the winning element

## Sound (Web Audio API — zero external files)

Unique synthesized sounds for: spin, reel stop, card deal, coin collect, plinko bounce, win fanfare, big win melody, loss
All sounds generated procedurally via oscillators

## Haptics

Light buzz on button presses and safe mine reveals
Medium buzz on dice rolls
Win pattern: [40, 20, 40, 20, 80] ms
Long buzz on loss

## UI

Dark mode toggle (🌙 / ☀️), saved to localStorage
Frosted-glass header with live coin counter
Animated page-position dots on the right edge
iOS-style bet selector, pill buttons, inset backgrounds
DM Sans font, Apple-style spacing and color tokens

