# OpenEvidence Panel for Anki

A modern Anki addon that integrates OpenEvidence directly into your Anki interface as a side panel.

## Features

- 📚 **Clean Toolbar Icon**: Open book icon in the top toolbar next to Sync
- 🎨 **Integrated Side Panel**: OpenEvidence opens as a docked panel on the right side of Anki
- 🎯 **Modern UI**: Minimalistic design with smooth hover effects
- 🔄 **Flexible Layout**: Dock, undock, or resize the panel as needed
- ⚡ **Quick Access**: Toggle the panel on/off with a single click
- 🔐 **Persistent Login**: Stay logged into OpenEvidence across sessions with automatic cookie storage
- ⌨️ **Smart Templates**: Keyboard shortcuts to auto-fill OpenEvidence with card content
- ✨ **Text Highlight Actions**: Select text on flashcards to instantly send to OpenEvidence
- ⚙️ **Customizable Settings**: Configure templates and quick action shortcuts

## Installation

### Method 1: Install from .ankiaddon file

1. Download the `openevidence_ai.ankiaddon` file from the [latest release](https://github.com/Lukeyp43/OpenEvidence-AI/releases)
2. Double-click the file, or open Anki and go to **Tools → Add-ons → Install from file...**
3. Select the downloaded `.ankiaddon` file
4. Restart Anki

### Method 2: Manual Installation

1. Download and extract the addon files
2. Copy the `openevidence_ai` folder to your Anki addons directory:
   - **Windows**: `%APPDATA%\Anki2\addons21\`
   - **Mac**: `~/Library/Application Support/Anki2/addons21/`
   - **Linux**: `~/.local/share/Anki2/addons21/`
3. Restart Anki

## Usage

1. After installation, you'll see a book icon (📖) in the top toolbar next to Sync
2. Click the book icon to open/close the OpenEvidence panel
3. The panel will appear docked on the right side of Anki
4. You can:
   - Resize the panel by dragging the separator
   - Undock the panel by clicking the pop-out button
   - Close the panel by clicking the X button or the toolbar icon

### 🔐 Persistent Login

**Stay logged in automatically!** The addon saves your OpenEvidence login session using cookies. Once you log in to OpenEvidence through the panel, you'll remain logged in even after closing and reopening Anki. No need to log in every time!

### ⌨️ Templates with Keyboard Shortcuts

**Quickly send card content to OpenEvidence** using customizable keyboard shortcuts. These shortcuts work when you're focused on the OpenEvidence search box.

The addon comes with **3 preset templates**:

**Preset 1: Standard Explain** - `Ctrl+Shift+S` (or `Cmd+Shift+S` on Mac)
- **Front side**: Sends your front with a polite prompt
  ```
  Can you explain this to me:

  [Your front]
  ```
- **Back side**: Sends both front and back
  ```
  Can you explain this to me:

  Question:
  [Your front]

  Answer:
  [Your back]
  ```

**Preset 2: Front/Back** - `Ctrl+Shift+Q` (or `Cmd+Shift+Q` on Mac)
- Sends only the front of your card on both sides
- Perfect for when you only want to search the front

**Preset 3: Back Only** - `Ctrl+Shift+A` (or `Cmd+Shift+A` on Mac)
- Front side: Sends nothing (empty)
- Back side: Sends only the back of your card
- Useful when you want to research just the back content

**Customize Templates:**
1. Click the **Settings** button (gear icon) in the panel's title bar
2. Click **Templates**
3. **Change preset shortcuts**: Click the edit button on any preset to change its keyboard shortcut
4. **Edit template content**: Modify what text gets sent for each template
5. **Create new templates**: Add your own custom templates with `{front}` and `{back}` placeholders
6. **Delete templates**: Remove any templates you don't need

You can change the keyboard shortcuts for the presets (like changing `Ctrl+Shift+S` to something else) or keep the defaults - it's completely customizable!

### ✨ Text Highlight Actions (Quick Actions)

**Instantly research any text from your flashcards!** While reviewing cards, highlight any text to show a floating action bar with two quick actions.

**How to use:**
1. **Select text** on any flashcard by clicking and dragging
2. A floating action bar appears above your selection with two options

#### Quick Action 1: Add to Chat
- **What it does**: Instantly sends the selected text directly to the OpenEvidence search box
- **Default shortcut**: `⌘F` (Mac) or `Ctrl+F` (Windows/Linux) - shown in the action bar
- **How it works**:
  - Click "Add to Chat" or press the shortcut key
  - The panel opens automatically (if closed)
  - Your selected text appears in the search box
  - You can edit the text or hit Enter to search immediately

#### Quick Action 2: Ask Question
- **What it does**: Opens an input field where you can type a question about the selected text, then sends both your question and the selected text to OpenEvidence
- **Default shortcut**: `⌘R` (Mac) or `Ctrl+R` (Windows/Linux) - shown in the action bar
- **How it works**:
  - Click "Ask Question" or press the shortcut key
  - Type your question in the input field
  - Press Enter or click the arrow button to submit
  - OpenEvidence receives: "Your question\n\nContext:\nSelected text"
  - The search is automatically submitted

**Example workflow:**
1. You're reviewing a card about "myocardial infarction"
2. Highlight the term "ST elevation"
3. Click "Ask Question" (or press `⌘R`)
4. Type "What causes this finding?"
5. Press Enter
6. OpenEvidence receives: "What causes this finding?\n\nContext:\nST elevation"
7. The search runs automatically!

**Customize Quick Action Shortcuts:**
1. Click the **Settings** button (gear icon) in the panel's title bar
2. Click **Quick Actions**
3. Click on either "Add to Chat" or "Ask Question" button
4. Press your desired key combination
5. Click **Save**

### ⚙️ Settings

Access settings by clicking the **gear icon** in the panel's title bar. The settings are organized into two main categories:

**Templates:**
- View all your keyboard shortcut templates
- Edit existing templates
- Create new custom templates
- Delete templates you don't need
- Customize keyboard shortcuts for each template

**Quick Actions:**
- Configure keyboard shortcuts for "Add to Chat" action
- Configure keyboard shortcuts for "Ask Question" action
- See your current shortcuts at a glance

## Requirements

- Anki 2.1.45 or later
- Internet connection (to access OpenEvidence.com)

## Credits

Created for medical students and professionals who want quick access to OpenEvidence while studying with Anki.

## License

Free to use and distribute.

## Support

For issues or questions, please visit our [GitHub repository](https://github.com/Lukeyp43/OpenEvidence-AI) or [open an issue](https://github.com/Lukeyp43/OpenEvidence-AI/issues).
