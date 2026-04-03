# JDZ Captcha

A PHP icon-based CAPTCHA library. Instead of distorted text or image recognition puzzles, users identify and select the icon displayed the least number of times in a randomized grid.

## How It Works

1. A grid of randomized icons is generated server-side using PHP's GD library
2. Icons are randomly rotated and flipped to prevent pattern recognition
3. The user selects the icon that appears the fewest times
4. The answer is validated server-side against session-stored data

## Features

- **Icon-based challenge** - No distorted text, no "select all traffic lights"
- **Pure PHP** - Built on the GD extension, no external services or API calls
- **CSRF protection** - Built-in token generation and validation
- **Honeypot field** - Hidden field to catch bots
- **Attempt limiting** - Configurable max attempts with cooldown timeout
- **Bot detection** - Click delay enforcement and hover detection
- **Session expiration** - Captcha data automatically expires
- **Single-use images** - Each generated image can only be requested once
- **Framework adapters** - Native PHP sessions, Symfony, and PSR-7/15 (Slim, Mezzio)
- **Fully configurable** - Theme, variant, grid size, security timing, messages, and more via YAML or code

## Requirements

- PHP >= 8.2
- GD extension

## Contact

This is proprietary software. For licensing, access, or more information:

- **Author:** Joffrey Demetz
- **Email:** joffrey.demetz@gmail.com
- **Website:** https://joffreydemetz.com
- **Project page:** https://jdz.joffreydemetz.com/jdzcaptcha
