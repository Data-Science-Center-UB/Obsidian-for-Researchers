
**Learning Objectives in this Exercise:**
- Transfer knowledge from Zotero to Obsidian.
- Process this knowledge using the **Zettelkasten method** in your Obsidian vault.
- This task requires that you have a basic understanding of how Zotero works.
- Note: This workflow is for reading and annotating PDFs in Zotero and then processing the annotations in Obsidian. If you have read a non-digital book or paper and have written the annotations in the notes section of the Zotero item, then complete the template as described in Step 6.

## Step 1: Prepare the Article in Zotero

Before creating your third *Zettel*, open **Zotero**.

1. **Add the article** from Exercise 03a as a PDF to your Zotero library.  
   **DOI:** [Feline gravity manipulation](https://doi.org/10.48550/arXiv.2503.22919)

2. **Highlight the following paragraphs and add the comments to them:**

   >**Paragraph:** "In 1922, the renowned British explorer Sir Archibald Whiskerton-Paws made a startling discovery in the longlost city of Mau-nekhet-ra. Hidden deep in the tomb of the enigmatic Pharaoh Felinhotep III, Whiskerton-Paws uncovered a series of remarkably preserved murals depicting cats in flight. These images, dating back to the 20th Dynasty (circa 1100 BCE), indeed the reverence of cats throughout the history of ancient Egyptian society, puzzled Egyptologists for decades [1]." <br>
   >**Comment:** The notion of cats in flight, especially within the context of space, playfully bridges ancient mythology with modern imagination. It evokes images of celestial felines gracefully navigating the cosmos, perhaps as guardians of the stars or as symbols of mystery and independence. This fusion of ancient reverence and contemporary fantasy underscores humanity's enduring fascination with cats and their enigmatic allure. #p1_literature_review
   >
   > **Paragraph:** "Cats indeed, uniquely in the animal kingdom, possess the ability to manipulate gravity." <br>
   > **Comment:** Cats can manipulate gravity. #p1_literature_review
   >
   >
   >**Paragraph:** "To this end, we propose a theoretical model, which we tentatively call Modified Feline Gravitational Dynamics or MOFEGD." <br>
   > **Comment:** MOFEGDE as a method should be used across the board; it is considered one of the author's most important discoveries. #p1_literature_review
   >
   >
   > **Paragraph:** Select Area: Figure 1, with the subtitle <br>
   > **Comment:** A flying cat circa 1100 BCE. #p1_literature_review

3. **Clean up the reference item:**
   - Remove all existing tags from the reference item (not the PDF).
   - Add the tag: `skimmed`

## Step 2: Create a Source Note in Obsidian

1. **Open Obsidian.**
2. **Press** `Ctrl + P`, then select:  
   ➔ *Zotero Integration: Add Source Note*
3. The *Quick Format Citation* window will open (via Zotero).
4. **Search for and select the reference:** *Toth, 2025*
5. **Press** `Enter`.

![10_screenshot_zotero_template](https://github.com/user-attachments/assets/ac48fcdc-740b-456c-ba87-23e971364746)



## Step 3: Turn the Knowledge into a "Zettel"

*Each paragraph and its comment can now become an individual "Zettel". If you have a lot of paragraphs, start with the most important ones. You can return later to process the rest.*

1. **Under the section containing the abstract, write the following link:**
	`[[flying_cats_acient_mythology_and_modern_aera]]`

2. **Click the link and create a new note** → **Press** ALT + E → **Select** "Zettel_Template" or **Press** ctr + p → "Templater: Open insert template modal → **Select** "Zettel_Template"

3. **Cut and paste the content in the "Zettel"** as shown below.  
	*(You don’t need to fill in the reference section — backlinks will cover this.)*
<br>

![11_screenshot_zettel_flying_cats_acient_mythology_and_modern_aera](https://github.com/user-attachments/assets/a55768a7-7c56-4d8b-8261-cc86f1467846)


5. **Repeate this for all of your paragraphs. Don't forget linking each Zettel to another. Move the Zettel (notes) you have just created to the "ZETTEL" folder.**
   **Note:** Copy the tag in the line "tags" without the #
7. **In the end it might look like this:**

![12_screenshot_toth_verzettelt](https://github.com/user-attachments/assets/9eebedcc-d96c-4655-966f-bdde79758eaa)


## Step 4: Use the Graph View for your Zettelkasten
*Click the graph view icon in the left toolbar to open it:*

![12_screenshot_open_graph_view](https://github.com/user-attachments/assets/a08351bd-5834-4796-a862-3b6a3b4c405b)

*At first, you'll see all your notes in the graph view. On the right side, you can open the graph view settings to filter which notes are displayed. In the search bar, type `path:ZEKA/ZETTEL`. Now, only the notes in your Zettelkasten will be shown.*
*Experiment with the settings and take a look at the documentation for more guidance: [Graph view - Obsidian Help](https://help.obsidian.md/plugins/graph)*

![13_screenshot_settings_graph_view](https://github.com/user-attachments/assets/80ad0cc2-82b4-4609-bbdf-5a53c374efc2)

*Here you can now see all the connections between the slips of paper. If you already have a lot of notes on a topic, you can consider whether it is worth creating an index page for the topic.*

*To display all notes for a specific tag, you can create a new group in the graph view settings and assign a specific color to the day.*
   
## Step 5: Create a Subject Index

Since you now have three "Zettel" related to the topic of cats — and you plan to continue working on this subject — this is a great moment to create a dedicated tag page.

1. **In your Obsidian vault**, navigate to your Zettelkasten folder (e.g., `ZEKA/ZETTEL`).

2. **Create a new note titled:** `[[cats]]`

3. **Click the link** to generate the new page.

4. **Inside the new "cats" page**, add a link to some of your cat-related Zettels.  
	For example: `[[cats_in_space]]`

*This link will serve as an **entry point** to all your notes about cats, helping you build a connected knowledge base around this theme.*

---

## Step 6 Annotations with the Note Function in Zotero (optional)

*If you have read a non-digital book or paper and have written the annotations in the notes section of the Zotero item, then complete the template as described:*

1. **Open Zotero Template in Obsidian.**
2. **Insert** `{{markdownNotes}}` as the last line in the template.

**Note:** If you want to customize the Zotero template, the “Zotero Integration: Data Explorer” (ctrl + p) is a helpful tool. Using a selected source note, you can see which commands you can use to transfer which element from Zotero to Obsidian.

