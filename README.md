# ImmersionKit Full Card Miner

A local Chrome extension that turns ImmersionKit sentence results into complete Anki cards.

It works directly with Anki through AnkiConnect and does not require an ImmersionKit account.

## What It Does

The extension adds an **Add full card to Anki** button beside each ImmersionKit result.

A card can include:

* Japanese sentence
* English translation
* Furigana
* Screenshot
* Sentence audio
* Source information
* ImmersionKit ID
* Page URL

Images and audio are downloaded into Anki's media collection, so the finished card does not depend on remote media links.

Each button works with its own ImmersionKit result, so the correct sentence, image, audio, and other information are captured.

## Install the Extension

These steps assume Anki and AnkiConnect are already installed and configured.
Do not click individual `.js`, `.css`, or `.json` files on GitHub. Those files
work together as one Chrome extension.

### 1. Download the extension from GitHub

1. Open the [ImmersionKit Full Card Miner GitHub page](https://github.com/chachaprince1/immersionkit-full-card-miner).
2. Near the upper-right part of the file list, click the green **Code** button.
3. In the menu that opens, click **Download ZIP**.
4. Wait for the download to finish. The file normally appears in your
   **Downloads** folder and is named `immersionkit-full-card-miner-main.zip`.

### 2. Unzip the download

#### macOS

1. Open **Finder**.
2. Click **Downloads** in the left sidebar.
3. Find `immersionkit-full-card-miner-main.zip`.
4. Double-click the ZIP file once. Finder creates a normal folder named
   `immersionkit-full-card-miner-main` beside it.
5. Drag that new folder somewhere permanent, such as **Documents**. Do not
   delete it after installing the extension.

#### Windows

1. Open **File Explorer**.
2. Click **Downloads** in the left sidebar.
3. Right-click `immersionkit-full-card-miner-main.zip`.
4. Click **Extract All…**.
5. Leave **Show extracted files when complete** checked, then click
   **Extract**.
6. Move the extracted `immersionkit-full-card-miner-main` folder somewhere
   permanent, such as **Documents**. Do not delete it after installing the
   extension.

### 3. Load the extracted folder into Chrome

1. Open Google Chrome.
2. Click the address bar at the top of Chrome.
3. Type `chrome://extensions` and press **Return** on macOS or **Enter** on
   Windows.
4. Turn on **Developer mode** using the switch in the upper-right corner.
5. Click **Load unpacked** in the upper-left corner.
6. In the folder window, select the extracted
   `immersionkit-full-card-miner-main` folder. Select the folder itself, not
   the ZIP file and not one of the files inside it.
7. Click **Select** or **Open**. If Chrome says it cannot find a manifest,
   you selected the wrong folder: go back and select the folder that directly
   contains `manifest.json`.
8. Chrome should add an **ImmersionKit Full Card Miner** card to the Extensions
   page.
9. Keep the extracted folder on your computer. Chrome loads the extension from
   that exact location every time it starts.

### 4. Confirm that it works

1. Open Anki Desktop and leave it running.
2. Open [ImmersionKit](https://www.immersionkit.com/) in Chrome.
3. Search for any Japanese word.
4. Look at one of the sentence results. You should see an
   **Add full card to Anki** button beside that result's Mining controls.
5. If the button is missing, return to `chrome://extensions`, find
   **ImmersionKit Full Card Miner**, click its circular-arrow **Reload** button,
   and refresh the ImmersionKit page.

## First-Time Setup

1. Open Anki Desktop and leave it running.
2. Open ImmersionKit, search for a word, and find any sentence result.
3. Click the small **⚙** button immediately beside
   **Add full card to Anki**. This opens **Anki settings**.
4. Open the **Deck** dropdown and click an existing Anki deck. To make a new
   deck, choose the new-deck option and type its name in **New deck name**.
5. Open the **Note type** dropdown. For the easiest setup, choose the bundled
   **ImmersionKit Full Card** note type.
11. Click **Save settings**.

The extension includes its own **ImmersionKit Full Card** note type and recommends it by default.

You can also use another Anki note type as long as it has appropriate fields for the information you want to save.

## Privacy

The extension runs locally.

It communicates with:

* ImmersionKit to retrieve sentence and media information
* AnkiConnect on your computer to create cards and store media

It does not send your card information to a separate extension server.
