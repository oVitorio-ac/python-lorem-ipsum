<p align="center">
 <a href="#-about-the-project">About</a> •
 <a href="#-features">Features</a> •
 <a href="#-layout">Layout</a> • 
 <a href="#-how-to-run-the-project">How to Run</a> • 
 <a href="#-technologies">Technologies</a> • 
 <a href="#-how-to-contribute-to-the-project">Contribute</a> • 
 <a href="#user-content--license">License</a> • 
 <a href="#-contributors">Contributors</a>
</p>

## 💻 About the project

The `pyloremgen` library is a Python package designed to easily generate Lorem Ipsum text and create PDFs with Lorem Ipsum content. Lorem Ipsum is placeholder text commonly used in the printing and typesetting industry.

## ⚙️ Features

- **Lorem Ipsum Paragraphs:** Generate Lorem Ipsum paragraphs effortlessly with the `paragraphs` method.

- **Random Words Generation:** Create a string of random words using the `words` method, allowing customization of the number of words.

- **Shopping List Generation:** Quickly generate a shopping list with randomly selected items using the `shopping_list` method.

- **PDF Generation:** Create PDF documents with Lorem Ipsum content using the `PDFGenerator` class. You can specify the number of pages and choose whether to include a cover page.

---

## 🎨 Layout

---

## 🚀 How to run the project

### Installation

To use the `pyloremgen` library, you first need to install it. You can install it using pip:

```bash
pip install pyloremgen
```

### Usage

#### Using `LoremIpsum` for Text Generation

Import the `LoremIpsum` class and create an instance:

```python
from pyloremgen.generator.lorem_text import LoremIpsum

lorem_generator = LoremIpsum()
```

##### Generating Paragraphs

To generate Lorem Ipsum paragraphs, use the `paragraphs` method:

```python
lorem_paragraphs = lorem_generator.paragraphs(paragraphs_numbers=3, size="medium", start_with_lorem_ipsum=True)
print(lorem_paragraphs)
```

This will generate three Lorem Ipsum paragraphs, starting with the default "Lorem ipsum" text.

##### Generating Words

To generate a string of random words, use the `words` method:

```python
lorem_words = lorem_generator.words(words_numbers=50)
print(lorem_words)
```

This will generate a string containing 50 random words.

##### Generating a Shopping List

To generate a shopping list of randomly selected items, use the `shopping_list` method:

```python
shopping_list = lorem_generator.shopping_list(items_count=5)
print(shopping_list)
```

This will generate a shopping list with 5 randomly selected items.

#### Using `PDFGenerator` for PDF Generation

Import the `PDFGenerator` class and create an instance:

```python
from pyloremgen.generator.lorem_pdf import PDFGenerator

pdf_generator = PDFGenerator()
```

##### Generating a PDF

To generate a PDF document, use the `generate_pdf` method:

```python
pdf_generator.generate_pdf(filename="example.pdf", num_pages=5, cover_page_count=True)
```

This will create a PDF named `example.pdf` with 5 pages, including a cover page.

### Examples

Here are some additional examples:

```python
# Example 1: Generating 2 paragraphs without starting with "Lorem ipsum"
lorem_text = lorem_generator.paragraphs(paragraphs_numbers=2, start_with_lorem_ipsum=False)

# Example 2: Generating a string of 20 random words
random_words = lorem_generator.words(words_numbers=20)

# Example 3: Generating a shopping list with 3 items
shopping_items = lorem_generator.shopping_list(items_count=3)

# Example 4: Generating a PDF with 3 pages and no cover page
pdf_generator.generate_pdf(filename="sample.pdf", num_pages=3, cover_page_count=False)
```

Feel free to customize the parameters based on your needs.

---

## 🛠 Technologies

- Python
- `reportlab` (for PDF generation)
- `pyloremgen` (for Lorem Ipsum text generation)

---

## Contribution ✨

Help the community make this project even more amazing. Read how to contribute by clicking **[here](https://github.com/oVitorio/.github/blob/main/CONTRIBUTING.md)**. I am convinced that together we will achieve incredible things!

---

## 📝 License

This project is licensed under the [MIT License](./LICENSE).

---

## 👨‍💻 Contributors

💜 A big thanks 👏 to these folks who brought this project from the realm of ideas to execution!

<table>
  <tr>
    <td align="center"><a href="https://github.com/oVitorio"><img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/88901960?v=4" width="100px;" alt=""/><br /><sub><b>Vitório Cavaleheiro</b></sub></a><br /><a href="https://github.com/oVitorio" title="github-oVitorio">👨‍🚀</a>
    </td> 
  </tr>
</table>

---