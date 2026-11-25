# Prescription Validator

A simple single-page web app for validating prescription input values for both eyes.

## What it does

- Accepts SPH, CYL, and Axis values for the left eye (OS) and right eye (OD)
- Checks each field against configured ranges
- Shows clear validation errors when values are missing, non-numeric, or out of range
- Displays a success message when all six inputs are valid

## Validation rules

- **SPH:** `-20.00` to `+20.00`
- **CYL:** `-6.00` to `+6.00`
- **Axis:** `1` to `180`

Missing values are rejected, and validation runs separately for each eye.

## How to use

1. Open `index.html` in a browser.
2. Enter SPH, CYL, and Axis for both eyes.
3. Click **Validate Prescription**.
4. Review the result message below the form.

## Project structure

- `index.html` — app markup, styling, and validation logic

## Notes

- The app is fully client-side and does not require a build step or external dependencies.
- Axis values are validated as whole numbers by the input field step, while the script enforces the configured range.
