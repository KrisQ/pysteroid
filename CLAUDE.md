# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

PysteRoid is a Python-based Asteroids game built with pygame. The project is in early development with a basic project structure established.

## Commands

### Development Environment
- **Python version**: 3.13 (specified in `.python-version`)
- **Package manager**: uv (evidenced by `uv.lock` file)
- **Install dependencies**: `uv sync`
- **Run the game**: `python main.py`

### Common Development Tasks
- **Add new dependencies**: Add to `pyproject.toml` dependencies array, then run `uv sync`
- **Check dependency lock**: Review `uv.lock` for current package versions

## Architecture

### Project Structure
- `main.py`: Entry point containing the main game loop initialization
- `constants.py`: Game configuration constants (screen dimensions, asteroid properties)
- `pyproject.toml`: Project configuration with pygame as the primary dependency

### Key Components
- **Game Constants**: Screen dimensions (1280x720), asteroid parameters (min/max radius, spawn rate)
- **Main Game Loop**: Currently minimal, prints basic game initialization info
- **Pygame Integration**: Set up as the primary game framework

### Development Notes
- The game is in early scaffolding phase with basic imports and configuration
- Constants are centralized in a dedicated module for easy configuration management
- Uses modern Python packaging with pyproject.toml and uv for dependency management