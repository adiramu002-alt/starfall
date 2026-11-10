# Starfall — Top-Down Space Shooter

## Repository
(https://github.com/adiramu002-alt/starfall/)

## Description
Starfall is a top-down arcade space shooter built in Python with Pygame. The
player pilots a ship, dodges and destroys waves of incoming enemies, and
survives as long as possible while the difficulty ramps up. It showcases
real-time animation, particle effects, and game-feel polish relevant to
digital arts and game design.

## Features
- Player ship with smooth keyboard movement
  - WASD/arrow keys move the ship; movement is clamped to the screen edges.
- Shooting mechanic
  - Spacebar fires projectiles upward; a cooldown controls fire rate.
- Enemy waves
  - Enemies spawn at random x-positions along the top and fall toward the
    player, increasing in frequency over time.
- Collision detection
  - Bullets destroy enemies; enemy/player contact costs a life.
- Particle explosions and visual juice
  - Destroyed enemies burst into fading particles (reusing my Digital Rain
    particle work), with optional screen shake for impact.
- Score and lives HUD
  - On-screen score counter and remaining lives rendered with Pygame fonts.
- Game states
  - Start screen, active play, and game-over/restart screen managed with a
    simple state variable.

## Challenges
- Collision detection between many bullets and enemies efficiently (likely
  using Pygame Rect and `colliderect`), which I need to research.
- Managing multiple object types (player, bullets, enemies, particles) cleanly
  with classes and lists without the code becoming tangled.
- Difficulty scaling and wave timing so the game feels fair but escalating.
- Game "juice" techniques (screen shake, particle feedback) to make it feel
  satisfying rather than flat.

## Outcomes
Ideal Outcome:
- A polished, playable space shooter with multiple enemy types, power-ups,
  particle explosions, screen shake, sound effects, and a start/game-over flow
  that feels like a real arcade game.

Minimal Viable Outcome:
- A single playable screen where the player moves, shoots, destroys one type of
  enemy, loses lives on collision, sees a score, and can restart after game
  over. A complete, working game loop even if visually simple.

## Milestones

- Week 1 (Nov 9–15)
  1. Set up repo, game window, player ship, and keyboard movement.
  2. Implement shooting (bullets fire and travel up the screen).

- Week 2 (Nov 16–22)
  1. Add enemy spawning and downward movement.
  2. Implement bullet–enemy and player–enemy collision detection.

- Week 3 (Nov 23–29)
  1. Add score, lives, and the HUD.
  2. Add particle explosions and start/game-over states.

- Week 4 (Nov 30–Dec 7) (Final)
  1. Polish: difficulty scaling, screen shake, colors, optional sound/power-ups.
  2. Final testing, cleanup, README, and submission.
