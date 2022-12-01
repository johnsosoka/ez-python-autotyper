# App Configuration

The ez-python-autotyper is configured via the `ez_autotyper_config.yml` which is specified by an environment
variable <tbd>. One of the primary goals of the application is to attempt to simulate human behavior while entering
repetitive commands; As such, some out-of-the-box functionality exists to delay command execution at random durations.

## Core Concepts

### Office Hours

Office hours are the range of hours that the bot will execute most typing jobs. The only exception is for a typing job
with a daily schedule--these jobs will execute around the time specified in the job spec.

### Timings & Behavior

### Profiles
DEBUG/PRODUCTION

### Logging & Metrics