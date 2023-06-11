# **PYPI PYTHON TRANSLATOR**
This is a translation application that allows you to translate text from one language to another using the Google Translate service. The program provides a user-friendly interface that automatically translates itself into the selected language.

---

## **Getting Started**

To use this program, you need to install the following libraries:

- `googletrans==4.0.0-rc1`
- `fuzzywuzzy`

You can install them by running the following command:

```bash
pip install googletrans==4.0.0-rc1
pip install fuzzywuzzy
```

## **Services**

The program requires access to Google services for translation. You don't need to write the available Google services into the `services.txt` file. it writes them for just information, if you are interested about services you can use `writeservices()` function in your code.

## **Language Examples**

This file contains a list of languages that can be used with the translation application. Each language entry is in the format `"<language code> - <country>"`. You can refer to this file when using the `init()` function.

For example:
- `init("en")` for English
- `init("tr")` for Turkish

Make sure to use the appropriate language code when initializing the translation application.


## **Function Reference**

### `writeservices()`

Writes all Google services to the `services.txt` file for using the transcript.

### `TRnslte(text: str, languages: str) -> str`

This is a self-translate function. It translates the given `text` into the specified `languages`.

### `init(langg: str) -> any`

This is the main function to start the translation application. It adjusts the interface based on the selected language and prompts the user for the desired exit language. After that, it performs the translations.

Please note that this program only runs with a valid `langg` value. If the value is not found in the `Language_Examples` file, the code will crash. Make sure to check the examples file for valid language codes.

## **Usage**

After setting up the necessary files and libraries, you can use the `init("language-code")` function to start the translation application. The program will guide you through the translation process, displaying the input and output languages, the translated text, and the translation accuracy.

Please make sure to enter valid languages and follow the instructions provided by the program.

**Note:** This program runs in an infinite loop until the user decides to exit. To terminate the program, use the appropriate exit command.

---
