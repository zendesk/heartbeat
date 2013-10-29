
Maintains a single interval, which is used to trigger tasks.

This is useful for something like:

- sending heartbeat messages
- performing cleanup operations occasionally

## API

### heartbeater.interval(ms)

Set the interval lenght for the heartbeat.

### heartbeater.start() / heartbeat.resume()

Start or resume the heartbeat.

### heartbeater.nextTimeout(millis)

Change the trigger time of the next timeout. For example, in order to guarantee that first heartbeat occurs within a shorter amount of time than average.

### heartbeater.add(cb)

Add a callback to the heartbeat actions.

### heartbeater.remove(cb)

Remove a callback from the heartbeat actions.

### heartbeater.pause()

Pause the heartbeat.

### heartbeater.clear()

Clear the heartbeat and all callback actions.
