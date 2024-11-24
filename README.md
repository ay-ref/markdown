# Markdown

## Instructions

### Items

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

  - if you have persian also

    ```shell
    pandoc *.md -o doc.pdf --pdf-engine=xelatex -V mainfont='Vazirmatn'
    ```
