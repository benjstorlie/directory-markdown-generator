# directory-markdown-generator
Generates a markdown document with a list of the directory's folders and files, with links. You can include comments that will be saved on refresh.

## Instructions
 * Run `node dir.js` in the terminal to generate a markdown document with a list of your directory's contents, including links. Run it again to refresh.
 * In VSCode, clicking those links will either open the file, or open the folder in the explorer sidebar.
 * In the generated document, you can add comments by adding a colon and space after the file link.
 * *Comments must be all on one line*
 * example `[fileName](path/to/fileName): Comment here.`
 * When you refresh the document, the comments will be included.
 * If there are any comments that weren't included, due to a deleted file or change in file structure, those comments will go in a section at the top for you to handle manually.
 * Edit `mdName` to make a custom name for your generated document.
 * Edit `ignore` and `ignoreContents` to list files or folders to ignore
 * Since it writes the markdown from scratch each time, you can't add anything else to the document or it won't be saved on refresh.

## Developer's Note

I am using this project as an exercise in making a complete npm module that someone could install. I have not finished yet, but I think this is small enough in scope that I can focus on just making a complete and functional project with really good documentation.

I do need to work on changing those parts that require the user to actually edit the script.
