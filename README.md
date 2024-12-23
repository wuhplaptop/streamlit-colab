
# Streamlit Colab

![Streamlit Colab](https://img.shields.io/badge/Streamlit-Colab-green.svg?style=for-the-badge)

Streamlit Colab is a command-line tool that allows you to run Streamlit applications with ngrok tunneling. This makes your local Streamlit app accessible via a public URL, which is especially useful for sharing your app with others or for testing purposes.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Documentation](#documentation)

---

## Introduction

**Streamlit Colab** enables you to easily share your Streamlit apps by exposing them to the web via ngrok. Whether you're collaborating on a project or showcasing your work, this tool provides a seamless way to make your apps accessible to the world.

---

## Installation

To install **Streamlit Colab**, use the following command:

```bash
pip install streamlit-colab
```

---

## Usage

Run your Streamlit app with ngrok tunneling using the following command:

```bash
stc <app.py> <ngrok_token> [port]
```

### Parameters:
- `<app.py>`: Path to your Streamlit application file.
- `<ngrok_token>`: Your ngrok authentication token.
- `[port]` (Optional): Custom port to run the Streamlit app on. Defaults to `8501` if not specified.

---

## Examples

### 1. Running with Default Port (8501)
Run your Streamlit app on the default port:

```bash
stc /path/to/your/app.py <your_ngrok_token>
```

### 2. Running with a Custom Port (e.g., 5005)
Specify a custom port, such as `5005`:

```bash
stc /path/to/your/app.py <your_ngrok_token> 5005
```

### 3. Using an Environment Variable for ngrok Token
Set your ngrok token as an environment variable and omit it from the command:

```bash
export NGROK_TOKEN=<your_ngrok_token>
stc /path/to/your/app.py
```

Override the port if needed:

```bash
stc /path/to/your/app.py 5005
```

---

## Documentation

For more detailed instructions and additional features, visit the [official documentation page](https://wuhplaptop.github.io/streamlit-colab/).

---

© 2024 Streamlit Colab. All rights reserved.
