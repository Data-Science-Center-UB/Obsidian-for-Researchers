
**Learning Objectives in this Exercise:**

- Writing a paper with the Zettelkasten.
- Query your Zettelkasten with the community plugin "Dataview"
- Revise your "Zettel" with the graph view and the random notes function.
## Step 1: Collecting Ideas for a Paper

1. **Open** `[[Publication Idea Collection]]` (created it exercise 04)
2. Here you can see our test query with the dataview plugin. **Replace `#test` with `#p1/lit_review` in the command.** (See "Backround Information Query's to Filter your Zettelkasten" below.) Now all the papers you have assigned to this tag are displayed. 
3. You can start writing the first draft of your paper. To do this, write `[[2025_paper_cats_gravity_v1]]` in your collection of ideas and create the note.
4. Here, you can start drafting the structure of your paper and begin collecting Zettels. For example, you might write something like this:

```
# Title: Cats in space. Cats that manipulate gravity

## 1. Introduction
[[picture_cats_in_space]]
[[picture_acient_cat_flys]]


## 2. Cats manipulate gravity

[[cats_manipulate_gravity]]

## References

```


## Step 3: Revise your Zettel 

*From time to time, it may be necessary to revise your Zettels. Click through your notes to create new connections, adjust existing ones, and identify topics that are suitable for a subject index page. By reading the "Output" section of your Zettels, you might also discover new ideas. You can use the graph view function for that*

**Random Note Function**
*Another option is the core plugin "Random Notes" (you'll need to enable it in the settings). A dice icon will then appear in the sidebar on the left. When you click the dice, you'll be shown random notes. The plugin pulls from all the notes in your vault, so depending on the ratio of Zettels to other notes, your chances of seeing more Zettels will increase or decrease.*

*But it can be a good way to rediscover Zettels you haven’t looked at in a while.*

## Backround Information Query's to Filter your Zettelkasten

*The Dataview plugin allows you to write queries and display your "Zettel's" in a specific, customizable way. This lets you view all notes with a particular tag (or all notes related to your project) with just a single click. For example:*

	```dataview 
	LIST 
	FROM "ZEKA/ZETTEL"
	AND #p1/lit_review
	```
*Idea: For example, you can add this to the “Ideas Collection Publication” note that you created in the “Learning Obsidian” exercises. You can then automatically display all notes that are relevant for this publication.*

*To explore additional query options, take a look at the documentation: [Dataview](https://blacksmithgu.github.io/obsidian-dataview/)*
