# ez-python-autotyper

An easy-to-use python autotyper for discord or any program requiring text input.

## Features

* Create & schedule autotyper jobs with a json file. No programming required to extend functionality!
    * Built in scheduler can handle many concurrent jobs
    * locked typing mechanism: A lock is acquired to type, so if two typing jobs execute at the same time one will
      complete before the other starts typing.
* Metrics! You can specify whether-or-not metrics should be collected for your job. These will be persisted to a target
  metrics.json
* Customizable behavior
  * Appear less bot like by randomly delaying when a scheduled command executes.
  * Establish "Office Hours" that the bot will execute during. Appear more _human-like_ by not executing commands 24/7
  * Control delay between commands being executed.

## Usage

### Configuration

### Running