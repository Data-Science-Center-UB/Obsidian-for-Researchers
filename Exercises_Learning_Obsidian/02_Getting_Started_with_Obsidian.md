# Getting Started with Obsidian
*(Duration approx. 10min)*

## Change the Color of Your Vault

Go to **Settings** → **Appearance** → First line **Base color scheme**. Change it into "dark", "light" or "adapt to system".

## Save and Back up Your Notes

- Obsidian automatically saves your notes as you type on your local device.
- Your notes are stored as Markdown (.md) files in the folder you selected for your vault.

**I highly recommend to implement a automatic back up of your Obsidian files. To protect yourself from data loss, find a second location for your data that is independent of your local device (e.g. a cloud).** Please find your individual solution here: [Back up your Obsidian files - Obsidian Help](https://help.obsidian.md/backup)

## Set yourself up
*You will see three columns on the start screen: a few icons and the list of your created notes or folders on the left, the currently open note in the middle and the graph view on the right.*

1. **Close the graph view (we will talk about this later).**
2. **Delete the note “Welcome” (right click on the note → delete).**

## Create Your First Note about Markdown Syntax

![1_screenshot_create_a_note](https://github.com/user-attachments/assets/30341720-8508-4d31-8b54-e3c3f6034f52)


1. **Click on the icon to create a new note or use the hotkey ctrl + n** (or on German keyboards strg + n)
2. **Rename the note to "Markdown Syntax** (your cheat sheet for learning Markdown syntax).
3. **Copy and add the following to the new note you just created.**

*In the provided text about Markdown three backticks are inserted at the beginning and at the end to display the raw, unformatted Markdown syntax.

![2_screenshot_backticks](https://github.com/user-attachments/assets/544806ba-16d2-4d09-8104-db5c4aa24147)

```markdown
*Markdown is a lightweight markup language that allows you to format text easily.*
   
### Markdown Syntax

- **Headings**: Use `#` for headings. For example, `# Heading 1`, `## Heading 2`, up to `###### Heading 6`.
- **Bold and Italics**: Use `*` or `_` for emphasis. For example, `*italic*` or `_italic_`, and `**bold**` or `__bold__`.
- **Lists**: Use `-` or `*` for unordered lists, and numbers for ordered lists.
- **Links**: Use `[text](URL)` for links.
- **Blockquotes**: Use `>` for blockquotes.
- **Code**: Use backticks `` `code` `` for inline code and triple backticks for code blocks.
- **Horizontal Rules**: Use `---`, `***`, or `___` for horizontal rules.
- **Checkbox**: Use `- [ ]` for checkboxes. You can check them by clicking in the box.
```

## Create a Folder "BACKEND"

*I recommend creating a folder where you have all the notes that are responsible for the infrastructure of your Obsidian Vault. This way you have them separate from your content notes. I use capital letters for the infrastructure pages/folders.*

1. **Create a folder and name it "BACKEND"

*Feel free to use different names for your folders and notes, but avoid changing them later. Changing names can cause conflicts, especially when working with templates.*

## Create the Note "CHANGELOG"

*When using Obsidian regularly, you'll adjust settings, troubleshoot issues, or add new features. Keeping track of these changes helps you remember what you did, how you fixed problems, and which features depend on each other. Documenting this process allows you to quickly revisit past solutions.*

*In computer science, such a record is called a "changelog". It is a file that lists changes, improvements, and bug fixes in chronological order, providing a clear overview of a project's development.*

1. **Create a note named "CHANGELOG" inside the folder "BACKEND" 
2. **Record where your Obsidian Vault is stored—you’ll likely need the file path often.**
3. **Insert the vault's location (e.g., `C:\Users\name\Desktop\ObsidianLocal\MyVault`).**
4. **Format the path to the folder like this:**
	``[Path Obsidian Vault](<C:\Users\name\Desktop\ObsidianLocal\MyVault>)``
5. **Now you created a link with which you can open your local folder where your .md files of your vault are stored.**

**Tips for Linking:**
- Remove any quotation marks.
- Folder and file names must not contain spaces—use `_` instead.

## Create the "ATTACHMENT" Folder

1. **Create a folder named "ATTACHMENT"** inside the "BACKEND" folder to store all the accepted file formats within your vault.
2. **Adjust the settings:**
	- Go to **Settings** → **Files and Links**
	- Change the attachment location as shown in the image.

![3_screenshot_attachment_folder_path](https://github.com/user-attachments/assets/109bc374-fd40-4a0e-bc3a-3ee766197da5)


3. **Test it:**
    - Create a note and insert an image or PDF via drag-and-drop or copy-paste.
    - The file should now be saved in the "ATTACHMENT" folder.
    - **Tip:** This only works for attachments in a note, not for attachments that you drag-and-drop on the left in your overview of notes and files.

**Obsidian supports the following file types:**

- **Markdown**: `.md`
- **JSON Canvas**: `.canvas` ([Learn more](https://jsoncanvas.org/))
- **Images**: `.avif`, `.bmp`, `.gif`, `.jpeg`, `.jpg`, `.png`, `.svg`, `.webp`
- **Audio**: `.flac`, `.m4a`, `.mp3`, `.ogg`, `.wav`, `.webm`, `.3gp`
- **Video**: `.mkv`, `.mov`, `.mp4`, `.ogv`, `.webm`
- **PDF**: `.pdf` 

See: [Accepted file formats - Obsidian Help](https://help.obsidian.md/file-formats)

## Core Plugin: Hotkeys

*Once you've familiarized yourself with Obsidian, hotkeys are a great way to navigate your vault. In the beginning it is not easy to learn and remember the new hotkeys. Obsidian helps you with that:*

**ctrl + p or strg + p → Open command palette**

*Here you can search for Hotkeys. To customize Hotkeys:*

**Settings → Hotkeys**

## Edit Changelog
Insert the following text into your note 'CHANGELOG' and include today's date.
```markdown
**dd/mm/yyyy**  
Settings for "Files and Links" have been changed. Attachments are now automatically stored in the ATTACHMENT folder. 
```
