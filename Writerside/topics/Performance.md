# Performance

This is a little more difficult to judge at this time. However, it's safe to assume the new version will perform radically better out-of-the-box even if we write terrible code. This is because

* We are on **.NET 9**, the latest SDK. By this fact alone we can expect **~30%** performance gains across the board.

* Memory is being fully consumed; there is no underlying OS to take up available memory and CPU.