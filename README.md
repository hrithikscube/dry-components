# dry-components

A lightweight React component library built with Tailwind CSS for styling. This library contains a collection of reusable components, making it easy to integrate into your projects.

## Features

- Built using **React** and **JSX**
- Styled with **Tailwind CSS**
- Simple and reusable component structure
- Customizable with Tailwind CSS classes

## Installation

First, install the library via npm:

```bash
npm install dry-components
```

## Usage

To use any component from the library, import it into your project like so:

```jsx
import { Input } from 'dry-components';
import { TextArea } from 'dry-components';
import { SelectInput } from 'dry-components';
import { PrimaryButton } from 'dry-components';
```

## Input Component Props

| Prop Name   | Type     | Required | Description                                                                                               |
|-------------|----------|----------|-----------------------------------------------------------------------------------------------------------|
| `value`     | `string` | Yes      | The current value of the input field.                                                                     |
| `name`      | `string` | Yes      | The name of the input field. Typically used for form handling.                                             |
| `type`      | `string` | Yes      | The type of the input (e.g., `text`, `password`, `email`, etc.).                                           |
| `handleChange` | `function` | Yes  | The function to handle the change event for the input field.                                               |
| `width`     | `string` | No       | Optional width of the input container, default is `w-full`. Accepts Tailwind CSS width classes.            |
| `label`     | `string` | No       | Placeholder text for the input field. If not provided, the placeholder will be empty.                      |

## TextArea Component Props

| Prop Name   | Type     | Required | Description                                                                                               |
|-------------|----------|----------|-----------------------------------------------------------------------------------------------------------|
| `value`     | `string` | Yes      | The current value of the text area.                                                                      |
| `name`      | `string` | Yes      | The name of the text area. Typically used for form handling.                                              |
| `type`      | `string` | No       | The type of the text area (not commonly used for `textarea`, but included for consistency).                |
| `handleChange` | `function` | Yes  | The function to handle the change event for the text area.                                                |
| `width`     | `string` | No       | Optional width of the text area container, default is `w-full`. Accepts Tailwind CSS width classes.        |
| `label`     | `string` | No       | Placeholder text for the text area. If not provided, the placeholder will be empty.                       |
| `rows`      | `number` | No       | Number of visible text lines. Defaults to 5.                                                               |

## SelectInput Component Props

| Prop Name   | Type       | Required | Description                                                                                               |
|-------------|------------|----------|-----------------------------------------------------------------------------------------------------------|
| `value`     | `string`   | Yes      | The current value of the selected option.                                                                 |
| `name`      | `string`   | Yes      | The name of the select input. Typically used for form handling.                                           |
| `options`   | `Array<{ value: string, label: string }>` | Yes | Array of option objects where each object has a `value` and a `label` property.                              |
| `handleChange` | `function` | Yes  | The function to handle the change event for the select input.                                               |
| `width`     | `string`   | No       | Optional width of the select input container, default is `w-full`. Accepts Tailwind CSS width classes.    |
| `label`     | `string`   | No       | Placeholder text for the select input. This will be shown as a disabled option when no option is selected. |

## PrimaryButton Component Props

| Prop Name | Type     | Required | Description                                                                                      |
|-----------|----------|----------|--------------------------------------------------------------------------------------------------|
| `label`   | `string` | Yes      | The text to display inside the button.                                                           |
| `onClick` | `function` | Yes    | The function to call when the button is clicked.                                                 |
| `width`   | `string` | No       | Optional width of the button container, default is `w-fit`. Accepts Tailwind CSS width classes. |
| `variant` | `string` | No       | The button style variant. Options include `outlined` and default (filled).                        |
