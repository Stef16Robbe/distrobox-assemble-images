# distrobox-assemble-images

Custom distrobox images

## Usage

distrobox assemble create --file {file}

See: https://distrobox.it/usage/distrobox-assemble/

Added updated fish prompt to show db name when active:

```fish
# ~/.config/fish/config.fish
function fish_prompt
    if test -n "$DISTROBOX_NAME"
        set_color green
        echo -n "(distrobox: $DISTROBOX_NAME) "
        set_color normal
    end

    # TODO: fix git branch etc.
    echo -n (prompt_pwd) '> '
end
```
