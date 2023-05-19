# Timestamps

## Scope

The following presents a standardised way for forming timestamps.

## Definition

Timestamps should be formulated as a string following this pattern according to the ISO 8601 standard:

```
yyyyMMddTHHMMSS
```

Here, `yyyy` standards for a four-digit year, e.g., `2023`, `MM` is the month, e.g., `01` for January, `dd` for the day of the year, e.g., `01` for the first of the month.

The `T` is a separator between date specification and time specification.

The time specification follows `HH` for hours, `MM` for minutes, and `SS` for seconds. As an example, `18:33:22` corresponds to 6 pm, minute 33 at second 22. When no second information is available, the `SS` information should be set to `00`.

### Generating the time stamp

To generate such a time stamp in Python, you can use the following command:

```
from datetime import datetime

timestamp = datetime.now().strftime("%Y%m%dT%H%M%S")
print(timestamp)
```

This code snippet retrieves the current date and time using datetime.now() and then formats it according to the desired pattern `%Y%m%dT%H%M%S`. The `%Y` represents the four-digit year, `%m` represents the two-digit month, `%d` represents the two-digit day, `%H` represents the two-digit hour in 24-hour format, `%M` represents the two-digit minute, and `%S` represents the two-digit second.

The output will be a string representing the current timestamp in the `yyyyMMddTHHMMSS` format, following the ISO 8601 standard.
