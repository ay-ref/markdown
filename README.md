# Markdown

## links

- [EMOJI CHEATSHEETS](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)

## setup

- BEST PLACE TO WRITE ***ENGLISH*** MARKDOWN (ALSO TO GET EXPORT) ARE **OBSIDIAN**, **VSCODE**!
- BEST PLACE TO WRITE ***PERSIAN*** MARKDOWN (ALSO TO GET EXPORT) IS **OBSIDIAN**!

## Instructions

### Items

- **EVERY INDENT INCLUDES MINIMUM 1 SPACE FROM END OF ITEM SPECIFIER OF PREVIOUS ITEM!**

- code:

    ```shell
    - item1
        - childitem1
            - item 1.1.1
        - childitem2
            - item 1.2.1
            - item 1.2.2
    ```

- output:

  - item1
    - childitem1
      - item 1.1.1
    - childitem2
      - item 1.2.1
      - item 1.2.2

### Inline Code

- code:

    ```shell
    `this is some code`
    ```

- output:

    `this is some code`

### Multiline Code

- code:

    ```shell
        ```python
        print('this is some python codee')    
        ```
    ```

- output:

    ```python
    print('this is some python codee')    
    ```

### Table

- code:

    ```md
        | table_col1 | table_col2 | talble_col3 | ... |
        | :--------  | :--------: | ----------: | --- |
        | table_1_1  | table_1_2  | table_1_3   | ... |
        | table_2_1  | table_2_2  | table_2_3   | ... |
        | ... | ... | ... | ... |
    ```

- output:

    | table_col1 | table_col2 | talble_col3 | ... |
    | :--------  | :--------: | ----------: | --- |
    | table_1_1  | table_1_2  | table_1_3   | ... |
    | table_2_1  | table_2_2  | table_2_3   | ... |
    | ... | ... | ... | ... |

### Link

- code:

    ```md
    [YOUR LINK TEXT](http://www.google.com)
    ```

- output:

[YOUR LINK TEXT](http://www.google.com)
  

### Image

- code:

    ```md
    ![image not shown text](./flame.jpg)
    ```

- output:

    ![image not shown text](./flame.jpg)

## Conversion

### To PDF

#### install obsidian (BEST WAY for english and persian!)

- copy your markdown codes and select export to pdf!

#### stackedit

- go to [LINK](https://stackedit.io/app#).
- paste your code.
- export to html.
- you can print your html!

#### VSCode Extension

- best way to do this is use from vscode extension `Markdown PDF`
  - first convert your markdown to html file!
  - then you can print your html to a pdf file!
  - even images print well in this approach!
  - you can even change html to make your own settings.

#### Pandoc

- for fast transmition also you can use `pandoc`
  - you can do multiple markdown to one pdf!

    ```shell
    pandoc *.md -o doc.pdf
    ```

    > again better technique is to first convert your `md` file to `html`,
    > by the command `pandoc *.md -o doc.html` and then convert it to `pdf`,
    > by the printing the web page to `pdf`!

  - if you have persian also

    ```shell
    pandoc *.md -o doc.pdf --pdf-engine=xelatex -V mainfont='Vazirmatn'
    ```

  - more complete command

    ```shell
    pandoc README.md -o out.tex --standalone && pdflatex out.tex && xreader out.pdf
    ```
