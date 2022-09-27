# logging

A janky, purely macro-based C logging "library".

- Should not be used as a permanent solution.
- Is used as a permanent solution in [Une](https://github.com/thechnet/une) and [Watchdog](https://github.com/thechnet/watchdog) (oops).

## How to use

1. Consider a robust alternative.
2. If you're still here:
- Clone this repository using `git clone --recurse-submodules https://github.com/thechnet/logging`.
- Do the following in **each of your compilation units** (or once in a header which you include everywhere):
  - `#define LOGGING_ID "<id>"`, where `<id>` is a short identifier for your project.
  - If your project uses wide strings: `#define LOGGING_WIDE`
  - `#include "<location>\include\logging.h"`, where `<location>` is the path to your clone of the repository.
- Refer to the source code for information on what kind of macros are available — the relevant ones start after the `/* LOGGING MACROS */` comment.
