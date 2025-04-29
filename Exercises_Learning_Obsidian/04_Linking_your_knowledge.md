## Linking your Knowledge
*(Duration approx. 10min)*

*Obsidians Bi-Directional Linking Feature:*
- **Enables users to create bi-directional links** between notes, fostering connections between ideas and forms a web of interconnected ideas.
- **Bidirectional linking means** that two notes are linked in both directions. If you set a link from note A to note B, you can also reach note A from note B. 

**Learning Objectives in this Exercise:**
- Linking your notes within Obsidian.
- Add a URL in your note.
- Create a link to a local file.
- Use the graph view.
- Use tags.

## Linking your notes

*I recommend building your vault as interoperable as possible. If you ever stop using Obsidian, you can use the .md files in another app which also use markdown syntax. This is the reason why I recommend to disable the wikilink format for internal links and set it to markdown format.*

**Settings** → **Files and links** → disable **Use Wikilinks** 

AND 

**Settings** → **Files and links** → enable **Automatically update internal links** 
*(It has nothing to do with interoperability, but since we are already here, we can do that as well. If you change the title of a note which is linked it will automatically update the internal links.)*

**Remember:** Add your changes in the settings to your CHANGELOG.
#### Exercise: Linking to other notes

*You found an important research article about cats, dogs and object recognition models in the previous exercise (Link: Use_the_Daily_Workflow). It's now afternoon and you have time to read the articles.*

1. **Write behind the task** "- [ ] Check literature [...]" (in your Daily Note, see exercise 2.2) the following:
```markdown 
[[Object Category Recognition]]
```
  *A link titled "Object Category Recognition" should now appear. You'll notice that its color is lighter compared to the other links. This is because the note for this header hasn't been created yet.*

3. **Click on the link**, and a new tab will open where Obsidian will automatically generate the note.
4. **Expand the right sidebar** → **click on backlinks** *Here, you can view all the backlinks to your note. Currently, you will see the mention in your daily note.*

![5_expand_right_sidebar](https://github.com/user-attachments/assets/3cd8e55e-9b86-4280-bada-87cb2a42969c)

![6_backlinks_for_note](https://github.com/user-attachments/assets/2ca37f3a-0cff-49b6-8985-0d20c93d3836)


5. You have read the article and found some really interesting facts which might be useful for your publication. **Copy the following in the note:**
```markdown
Pets in Clothes: The research team found that one of the common issues with the images collected for their dataset was pets wearing clothes. The article mentions that images of pets dressed up were often discarded, which implies that while some owners may enjoy dressing their pets, it complicates the task of accurately identifying their breed. 
Source: [Cats and dogs | IEEE Conference Publication](https://ieeexplore.ieee.org/abstract/document/6248092) 
[[Publication Idea Collection]]
```
6. **Go to the note** "Ideas Collection Publication" by clicking the link.
7. *In the right sidebar you can see all the places where you had ideas for your publication (pretend for a moment that there are more) and you can start planning your paper.*

### Graph View

*The graph view is a great tool for getting an overview of your linked notes. You can visualize your knowledge with just one click. For more information check out the documentation: [Graph view](https://help.obsidian.md/plugins/graph)*

1. **Left sidebar** → **Click on graph view icon**

*There are many options to customize the graph view. Please take a look at the documentation. The local graph, the filter and the groups can be great tools to show you only certain links instead of all your Notes.*

### Linking a local file

*It is also possible to write a link in a note in Obsidian that allows you to open a file from your computer. You need to insert a path to a file on your local device into the following link. You can find the path by right-clicking on a file and selecting "Copy as Path". Usually there will automatically will insert double quotation mark. You have to replace them with <  > We have already applied this in task 02 in our CHANGELOG.*

```markdown
[filename](<absolute-path>)
```

*If you change the name of your local file on your local device (and with it the path to the file) the link in Obsidian will not automatically be updated.*

### Using Tags

*You can structure your knowledge by using #tags*

*In this vault, there are two ways to query tags:*
1. You can use the **search bar** on the left (icon magnifier).
2. You can **write a query and use the Dataview plugin** you installed in the exercises before. Here is an example for a list query of the tag #test . Copy the following into the note "Publication Idea Collection". After pressing the Enter key, Obsidian automatically transfers the command to a list. To see the command again move with your courser to the field where you see the list and click on </>

       ```dataview
       LIST
       FROM #test
       ```
*To see a list add the tag `#test` to different notes in your vault (you can delete the tags afterwards).*

You can write many different kind of querys with the Dataview plugin. Check out the documentation: [Dataview](https://blacksmithgu.github.io/obsidian-dataview/)
