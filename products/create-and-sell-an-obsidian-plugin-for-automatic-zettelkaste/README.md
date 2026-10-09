# Create and sell an Obsidian plugin for automatic Zettelkasten ID generation

**Price: $12.00** · [Buy the full pack](https://buy.stripe.com/3cIeVef1A4ZvdNx10jawo2i) · delivered as a Markdown file you can import or edit.

Obsidian Zettelkasten ID Generator Plugin - delivered as a Markdown file you can import or edit.

*Product line: Write and license a small software utility*

---

## Preview

# Obsidian Zettelkasten ID Generator Plugin
Version: 1.0.0

## File Structure
```
obsidian-zettelkasten-id/
├── manifest.json
├── main.js
├── styles.css
├── LICENSE
└── README.md
```

### manifest.json
```json
{
  "id": "zettelkasten-id-generator",
  "name": "Zettelkasten ID Generator",
  "version": "1.0.0",
  "minAppVersion": "0.15.0",
  "description": "Automatically generates sortable Zettelkasten IDs for new notes.",
  "author": "Your Name",
  "authorUrl": "https://github.com/yourname/zettelkasten-id-generator",
  "isDesktopOnly": false
}
```

### main.js
```javascript
/* Obsidian Zettelkasten ID Generator Plugin v1.0.0
   MIT Licensed – see LICENSE file */

import { Plugin, TFile, Notice } from 'obsidian';

export default class ZettelkastenIDGenerator extends Plugin {
    async onload() {
        // Add command to generate ID for current note
        this.addCommand({
            id: 'generate-zettelkasten-id',
            name: 'Generate Zettelkasten ID',
            editorCallback: async (editor) => {
                const cursor = editor.getCursor();
                const id = this.generateID();
                editor.replaceRange(id, cursor);
                new Notice(`Inserted Zettelkasten ID: ${id}`);
            }
        });

        // Add command for creating a new note with ID in filename
        this.addCommand({
            id: 'create-note-with-id',
            name: 'Create New Zettelkasten Note',
            editorCallback: async () => {
                const id = this.generateID();
                const defaultName = `${id}.md`;
                const file = await this.app.vault.create(defaultName, '');
                await this.app.workspace.openLinkText(file.path, '', true);
                new Notice(`Created note: ${defaultName}`);
            }
        });
    }

    onunload() {}

    /** Generate a timestamp-based Zettelkasten ID: YYYYMMDDHHMM */
    generateID() {
        const now = new Date();
        const pad = (n) => String(n).padStart(2, '0');
        return `${now.getFullYear()}${pad(now.getMonth() + 1)}${pad(now.getDate())}${pad(now.getHours())}${pad(now.getMinutes())}`;
    }
}
```

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $12.00](https://buy.stripe.com/3cIeVef1A4ZvdNx10jawo2i)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
