# ez-python-autotyper

An easy-to-use python autotyper for discord or any program requiring text input.

## Features

* Create & schedule autotyper yml based typing jobs which can execute a series of text entry & key press commands. No programming required to add functionality!
    * Built in scheduler can handle many concurrent jobs
    * locked typing mechanism: A lock is acquired to type, so if two typing jobs execute at the same time one will
      complete before the other starts typing.
* Metrics! You can specify whether-or-not metrics should be collected for your job. These will be persisted to a target
  metrics.json
* Customizable behavior
  * Appear less bot like by randomly delaying when a scheduled command executes.
  * Establish "Office Hours" that the bot will execute during. Appear more _human-like_ by not executing commands 24/7
  * Control delay between commands being executed.

## Example Job Spec
The following two job specs have the same functionality. 

### Job With Minimal/Default Settings

```yaml
JOB_NAME: work
INSTRUCTIONS:
- TYPE_TEXT: "!work"
- PRESS_AND_RELEASE: enter
```

### Job with All Settings

```yaml
JOB_NAME: work
RESPECT_OFFICE_HOURS: true
DELAY_COMMAND_EXECUTION: true
COLLECT_METRICS: true
SCHEDULE_PROFILES:
  PRODUCTION:
    TYPE: Hourly
    INTERVAL: 1
  DEBUG:
    TYPE: Minutes
    INTERVAL: 1
INSTRUCTIONS:
- TYPE_TEXT: "!work"
- PRESS_AND_RELEASE: enter

```

## Usage

### Configuration

### Running