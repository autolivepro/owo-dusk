# Pterodactyl / Bot-Hosting notes

This fork is intended for a headless Linux/Pterodactyl container.

- Entry point: `uwu.py`
- Do not set `install.bat` as the Python file.
- The desktop Tkinter popup import has been disabled because headless containers
  generally do not provide `libtk8.6.so`.
- If the panel has a `BOT PY FILE` variable, set it to `uwu.py`.
