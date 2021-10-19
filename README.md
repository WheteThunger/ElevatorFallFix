## Features

- Fixes an issue introduced in the October 2021 Rust update where players get unparented from elevators while moving quickly

## How the bug works

The bug happens when the elevator is moving quickly, while the player is either touching the edges of the lift or moving around. While the lift is moving up quickly, the player may fall through the elevator. While the lift is moving down quickly, the player may not be able to keep up with the elevator and start falling toward it. Either case can cause flyhack detection or fall damage.

The bug only happens with deployable elevators, not static elevators. It also doesn't cause any impact for vanilla elevators speeds because they are so slow that the player will simply be reparented in a short time.

## Caution

This might unintentionally reintroduce past elevator exploits.
