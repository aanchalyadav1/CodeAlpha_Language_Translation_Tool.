# Language Translation Tool

This repository contains a simple language translation tool that translates text from English to French using the `googletrans` library. The tool is implemented in a Google Colab notebook for easy use and accessibility.

## Installation

To use the translation tool, you need to install the `googletrans` library. The installation can be done directly in the Google Colab environment using the following command:

```python
!pip install googletrans==4.0.0-rc1
```

## Usage
**1. Clone the Repository:**

- Clone this repository to your local machine using:
```git
git clone https://github.com/SouhailMah/CodeAlpha_Language_Translation_Tool.git
```
**2. Open Google Colab:**

- Go to Google Colab.

- Open the `CodeAlpha_Language_Translation_Tool.ipynb` notebook from the cloned repository.

**  3. Run the Notebook:**

-Install the `googletrans` package by running the first cell in the notebook:
```python
!pip install googletrans==4.0.0-rc1
```

-Follow the instructions in the notebook to input the text you want to translate and view the translated text.

### Example Code
Here is a sample code snippet that demonstrates how to use the translation tool in Google Colab:
```python
# Install the googletrans package
!pip install googletrans==4.0.0-rc1

# Import the necessary library
from googletrans import Translator

# Define the translation function
def translate_text(text, src='en', dest='fr'):
    translator = Translator()
    try:
        translation = translator.translate(text, src=src, dest=dest)
        return translation.text
    except Exception as e:
        return f"Error: {e}"

# Input text to translate
text_to_translate = "Hello, how are you?"

# Translate the text
translated_text = translate_text(text_to_translate)

# Print the translated text
print(f"Translated text: {translated_text}")
```

## Contributing

Contributions are welcome! If you have any suggestions or improvements, please create a pull request or open an issue.

## License

This project is licensed under the MIT License.

## Contact

If you have any questions or feedback, feel free to reach out to me at [souhail.mah@gmail.com].




