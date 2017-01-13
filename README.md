# ngErrors

![ngErrors](https://github.com/utecht/ngErrors/raw/master/example.png)

This is a simple Angular2 "module" for handling displaying errors for the user.  It is currently combined into a single file for portability but could be split back into multiple files if that is your preference.

## Installation

Drop into place and add ErrorService to your providers and ErrorComponent to your declarations.  Then drop the <app-error></app-error> someone higher up in your templates.  This requires bootstrap4 for proper styling.

## Usage

The ErrorService has a function announceError(title: string, description: string, severity: number).  Calling this function from anywhere will cause a new error to appear with color determined by the severity.

| Severity | Bootstrap Class |
| -------- | --------------- |
| > 2 | info |
| 2 | warning |
| >2 | danger |

