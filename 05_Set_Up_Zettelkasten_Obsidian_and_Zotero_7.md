
*This manual is written for **Zotero 7.0***

*The following plugins are used:*
- *Zotero: Better BibText*
- *Obsidian: Zotero Integration*

*Following workflow is possible with this set up:*
- *Read and annotate your texts in Zotero.*
- *Import tags, bibliographic data, abstract, link to the Zotero file, annotations and comments in the annotations in Obsidian.*
- *Set up for Zettelkasten-Method (Niklas Luhmann)*

*The naming convention is based on the exercises 1-4 in this GitHub Repo and also the settings in this exercises might be important for this exercise. Feel free to adapt this to your needs.*

## Settings in Zotero

*With the Zotero plugin Better BibTex you can manage your bibliographic data more easily if you use a Markdown editor. The plugin automatically generates a citation key that follows a form you have selected. In Obsidian our literature note will automatically named with this citation key.*

**Download the .xpi file from the GitHub repository** [Better BibTeX for Zotero](https://github.com/retorquere/zotero-better-bibtex/releases/tag/v7.0.17)

[Click here for the documentation of Better BibTex](https://retorque.re/zotero-better-bibtex/index.html)

Install Better BibTex:
**Tools → Plugins → Settings → Install Plugin from file → select .xpi file → click open → restart zotero**

Customize Better BibTex:
**Edit → Settings → Better BibTex → Citation key → insert:**

```
"z." + authEtal2(creator = "*", initials = false, sep = ".").fold + year
```
**Output:** z.Author.etal.year

*I use the prefix “z.” so that I can easily distinguish between source notes from Zotero and source notes that I have only created in Obsidian.*

*Please visit the plugin documentation if you would like to create a different cite key.*

**Display citation key:**
**Right-click on bar "Titel | Creator | Attachment" → select citation key**
*Now you can see the citation key for each of your reference.*

→ **Document all settings in your CHANGELOG**
## Settings in Obsidian

**Community plugins → Browse → Zotero Integration by mgmeyers → Install → Enable**

**Open Zotero Integration Settings → set the "Note Import Location" → Enable "Open the created note after import"

*For Zettelkasten (see next exercise):*

**Create a folder** named "ZEKA" → **Create inside the folder** "Source_Notes" and "ZETTEL" → set the Note Import Location to "ZEKA/SOURCE_NOTES"

→ **Document all settings in your CHANGELOG**
## Settings in Obsidian and Zotero

*Synchronize the citation format*

*Zotero:* 
**Settings → Cite → Select your Citation Format and remember it**

*Obsidian:* 
**Citation Format → Add Citation Format → Select the same as in Zotero

**Import Formats → Add Import Format  
	Name:** "Add Source Note" 
	**Output Path:** ZEKA/SOURCE_NOTE/{{citekey}}.md
	**Image Output Path:** BACKEND/ATTACHMENT/{{citekey}}/
	**Template File:** BACKEND/TEMPLATES/Zotero_Template.md
	**Bibliography Style:** Select the same citation format like before

→ **Document all settings in your CHANGELOG**
## Zettelkasten Set Up

1. **Zotero Template**

*In Obsidian:*
**Add in Folder BACKEND/TEMPLATES** new note "Zotero_Template" and copy the following template in it (or use/build your own):

```
---
tags: {% if allTags %}{{allTags}}{% endif %}
created: {{importDate|format("YYYY-MM-DD")}}
---


### Titel: {{title}}

**Authors:** {{authors}}

**Reference:** {{bibliography}}
**Zotero Link:** {{pdfZoteroLink}}

> [!NOTE]- Abstract
> {{abstractNote}}


{% for annotation in annotations -%} 
{%- if annotation.annotatedText -%}*{{annotation.annotatedText}}*([p.{{annotation.pageLabel}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.pageLabel}}&annotation={{annotation.id}}))
{% endif %}{% if annotation.imageRelativePath %}![[{{annotation.imageRelativePath}}]]{% endif %}
{% if annotation.comment %}{{annotation.comment}}{%- endif %} 
{% if annotation.hashTags %}{{annotation.hashTags}}{%- endif %} 

{% endfor %}
```

*The template generates this output:*

![](7_screenshot_zotero_template.png)

→ **Document all settings in your CHANGELOG**


2. **Zettel Template**

*In Obsidian:*
**Add in Folder BACKEND/TEMPLATES** new note "Zotero_Template" and copy the following template in it (or use/build your own):

```
---
Created: <% tp.file.creation_date() %>
tags:
---
### Input

### Reference

### Output

### Link

```

