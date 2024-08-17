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
