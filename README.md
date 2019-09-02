# whatsapp_chat_dump
A small script for listing and exporting WhatsApp chat sessions. Exporting group chats is not supported (yet).
This is a personal project and will be extended and optimized in the future.

## Important
This project requires the following modules:
* Docopt
* Pandas
* Yattag

Furthermore, the ChatStorage.sqlite file (the WhatsApp Chat database) must be in the same directory.

## Usage
```
Usage:
    wad.py dump_chats [--cd | <output>] [--all | --custom <sid>...]
    wad.py sessions [(find (--name <name> | --number <number>))] [--sort]
    wad.py -h | --help

Examples:
    wad.py dump_chats --custom 7 11 420
    wad.py dump_chats "C:/Users/pixel3rr0r/Documents/Exported Chats"
    wad.py sessions --sort
    wad.py sessions find --name "Niels Bohr"

Options:
    --cd               Exports chats to the current directory (Default)
    --all              Exports every chat (Default)
    --custom           Exports one or more (seperated by space) given chat sessions
    --name             Finds all chat sessions with the given name
    --number           Finds all chat sessions with the given number
    --sid              Finds all chat sessions with the given Session-ID
    --sort             Sorts the list alphabetically
    -h --help          Shows this help message
```

## TODO
- [X] Add find function
- [ ] Add group chat support
- [ ] Add macOS support
