
# Doxygen Notes

## 1. Introduction

Doxygen is an open-source documentation generator for programming languages such as C, C++, Python and Java.

It extracts information from special comments in source code to generate reference manuals.

## 2. Key Features

- Extracts function, class and module documentation.
- Generates cross-referenced code.
- Generates call graphs and inheritance diagrams.
- Supports Markdown and LaTeX formulas.
- Supports code examples.

## 3. Comment Syntax

Doxygen uses specially formatted comments.

```cpp
/**
 * \brief Brief description of function.
 *
 * Detailed explanation.
 * \param x Parameter description.
 * \return Return value description.
 */
int myFunction(int x);
```

## 4. Common Doxygen Tags

| Tag | Purpose |
|---|---|
| `\brief` | Short description |
| `\param` | Parameter description |
| `\return` | Return value |
| `\author` | Author information |
| `\version` | Version |
| `\see` | Related reference |
| `\note` | Additional notes |

## 5. Configuration File

Create a configuration file using:

```bash
doxygen -g Doxyfile
```

Run Doxygen using:

```bash
doxygen Doxyfile
```

## 6. Output Formats

Doxygen supports:

- HTML
- LaTeX/PDF
- RTF
- XML
- Docbook
- man pages

HTML is the default output format.

### Configuration Options

```text
GENERATE_HTML = YES
GENERATE_LATEX = YES
GENERATE_RTF = NO
GENERATE_XML = NO
```

## 7. Basic Doxygen Workflow

1. Write specially formatted comments in source code.
2. Create or edit the configuration file.
3. Run Doxygen.
4. Browse the generated documentation.

HTML output can be opened using:

```text
html/index.html
```

## 8. Mini-Project

The PPT demonstrates the following practical exercise:

1. Download and install Doxygen.
2. Comment a small C++ or Python codebase.
3. Generate HTML output.
4. Open `html/index.html`.
5. Explore diagrams and cross-references.

## 9. Best Practices

- Document the purpose of functions.
- Keep brief and detailed descriptions distinct.
- Document public APIs and modules.
- Use consistent tags and layout.
