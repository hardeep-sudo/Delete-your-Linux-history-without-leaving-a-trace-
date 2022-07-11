# Delete-your-Linux-history-without-leaving-a-trace

So this is a way to delete a line from the history file without actually leaving this trace behind. The solution to this problem is this;

# history -d $((HISTCMD-1)) && history -d [line entry number]

Of course you could also use this command to run another command without it getting logged to the history file if you were so inclined;

# history -d $((HISTCMD-1)) && [type_your_command_here_and_execute]
