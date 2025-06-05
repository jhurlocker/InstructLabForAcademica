# 
# :bulb: Spaces and indentation matter in YAML. 

If you're creating your files using the command line interface (CLI), you'll need to use Markdown (MD) formatting within the qna.yaml file. Please note that formatting is crucial in this context. It's highly recommended to refer to an example file and closely follow its indentation and use of tabs or spaces to ensure consistency and correctness.

- Use two spaces to indent.
- Don't use tabs!
- Do not have trailing spaces at the end of a line.
- Each example in seed_examples begins with a dash (-). Place this dash in front of the first field (question or context). The remaining keys in the example should not have this dash.
- Some special characters such as a double quotation mark (") and an apostrophe or single quotation mark (') need to be escaped with backslash. This is why some of the lines for keys in the example YAML start the value with the pipe character (|) followed a new line and then an indented multi-line string. This character disables all of the special characters in the value for the key.
- You might also want to use the pipe character (|) for multi-line strings.
- Consider quoting all values with double quotation marks (") to avoid surprising YAML parser behavior (e.g., Yes answer can be interpreted by the parser as a boolean of True value, unless "Yes" is quoted.)


## [See yaml-multiline.info for more info](https://yaml-multiline.info/)

