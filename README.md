# Mac Compose Key Bindings

These are the default X11 compose key configurations (from the en.US-UTF8 locale) translated to Mac key bindings. They can be installed for use with Karabiner Elements using the instructions at cmloegcmluin/compose2keybindings. 


For some reason, I found that the Karabiner rule suggested my cmloegcmluin doesn't work properly with BBEdit 16 and later, but the following rule can be used instead and seems to work perfectly:

```
{
    "description": "MacCompose",
    "manipulators": [
        {
            "from": {
                "key_code": "right_option",
                "modifiers": { "optional": ["any"] }
            },
            "to": [
                {
                    "key_code": "non_us_backslash",
                    "modifiers": ["left_shift", "left_option"],
                    "repeat": false
                }
            ],
            "type": "basic"
        }
    ]
}
```
