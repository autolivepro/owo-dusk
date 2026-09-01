# Pterodactyl / Bot-Hosting notes

This fork is intended for a headless Linux/Pterodactyl container.

## Entry point
`uwu.py`

`uwu.py` now changes its working directory to the project directory automatically,
so relative paths such as `config/global_settings.json` and `utils/data/db.sqlite`
work even when Pterodactyl starts the file from `/home/container`.

## Recommended panel settings

If the project files are inside `/home/container/owo-dusk/`:
- BOT PY FILE: `owo-dusk/uwu.py`
- REQUIREMENTS FILE: `owo-dusk/requirements.txt`
- START BASH FILE: blank

Do not set `install.bat` as the Python file.

The desktop Tkinter popup import is disabled for headless Linux containers.
