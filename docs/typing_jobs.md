# Typing Jobs

Typing jobs are generated from a yaml `job spec`. By default jobs come with some behavior, most of which can be
overridden in fields within the spec. The only mandatory entries for the job spec are `JOB_NAME` and an `INSTRUCTIONS`
set with at least 1 command.

## Valid Commands

| Command           | Details                                                                                                                                                                      |
|-------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| TYPE_TEXT         | The `TYPE_TEXT` command will type the text specified in the value. It will press keys at a rate of `text_write_interval` seconds specified in the `ez_autotyper_config.yml`. |
| PRESS_AND_RELEASE | `PRESS_AND_RELEASE` will press and release a specific key. Vew supported keys below.                                                                                         |
| WAIT              | The `WAIT` command will simply wait for the amount of seconds specified in the key                                                                                           |
