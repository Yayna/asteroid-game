# Asteroids

A classic Asteroids clone built in Python with [pygame](https://www.pygame.org/).

## Requirements

- Python >= 3.13
- pygame 2.6.1

## Installation

This project uses [uv](https://github.com/astral-sh/uv) for dependency management.

```bash
uv sync
```

## Running the Game

```bash
uv run main.py
```

## Controls

| Key     | Action          |
| ------- | --------------- |
| `W`     | Move forward    |
| `S`     | Move backward   |
| `A`     | Rotate left     |
| `D`     | Rotate right    |
| `SPACE` | Shoot           |

## Gameplay

- Asteroids spawn from the edges of the screen and drift across.
- Shoot an asteroid to split it into smaller pieces; the smallest pieces are destroyed entirely.
- Colliding with any asteroid ends the game.

## Project Structure

- [main.py](main.py) — game entry point and main loop
- [player.py](player.py) — player ship logic
- [asteroids.py](asteroids.py) — asteroid sprite and splitting logic
- [asteroidfield.py](asteroidfield.py) — asteroid spawner
- [shot.py](shot.py) — projectiles
- [circleshape.py](circleshape.py) — base sprite class with collision
- [constants.py](constants.py) — tunable game constants
- [logger.py](logger.py) — JSONL event/state logger
