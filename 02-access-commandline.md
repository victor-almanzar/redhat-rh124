# Access the Command Line

## Execute Commands in Bash Shell

The following operates can be placed between commands:

### `whoami`

Find out what user is currently logged in

### `su -`

Substitute your user ID for another user. replace `-` with a users name, if you use `-` you will substitute your user ID with that of roots.

### `;`

Unconditional command execution, they can all execute independently.

### `&&`

Conditional command execution, if command a executes, then b can execute.

### `||`

if command fails to executes, then b can executes.

### `^`

look up and replace word with word, example:

```bash
ls /usr
^usr^tmp 
```

this executes ls `ls /tmp`

### `sudo`

Run command as a privileged user (the permissions of root)

### `!!`

Run the previous command, useful for when you forget sudo. can also be placed before a command (or option)

### `date`

Returns time and date.

- `date +%R` time
- `date +%D` date
- `date +%F` date in ISO 8601

### `History`

Shows the command you've used so far

### `!{number}`

After you run `history` you can select a command you've previously ran by selecting its ID and typing it after the `!`.

example: you've previously ran `clear`. `history` says it has an ID of 5. `!5` runs `clear`.
