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

## Install

### 1. Prepare Anki

Keep Anki open and make sure **AnkiConnect** is installed and running on port **8765**.

### 2. Install the Chrome extension

In Chrome:

1. Open `chrome://extensions`
2. Turn on **Developer mode**
3. Click **Load unpacked**
4. Select the extension folder

### 3. Open ImmersionKit

Each search result should now have an **Add full card to Anki** button beside its Mining controls.

## First-Time Setup

The first time you use the extension:

1. Choose an Anki deck or create a new one.
2. Choose your Anki note type.
3. Review the field mappings.
4. Save the settings.

The extension includes its own **ImmersionKit Full Card** note type and recommends it by default.

You can also use another Anki note type as long as it has appropriate fields for the information you want to save.

## Adding a Card

Click **Add full card to Anki** beside the sentence you want.

By default, the extension shows a preview before adding the card. You can review or edit the:

* Japanese sentence
* Translation
* Reading
* Source title

The preview also checks whether the screenshot and audio were found.

If either is missing, the extension warns you before allowing the card to be added.

If you do not want to see the preview each time, you can turn it off in Settings.

## After Adding a Card

Once the card has been added, the button changes to:

**View in Anki**

Clicking it opens Anki's Browser and selects that exact card.

The same thing happens if the extension discovers that the ImmersionKit result is already in Anki. Instead of creating a duplicate, it gives you **View in Anki**.

## Settings

Click the **⚙** beside an Add button to open Settings.

From there you can change:

* Anki deck
* Note type
* Field mappings
* AnkiConnect URL
* Card preview preference
* Which Anki add button appears on ImmersionKit

Your choices are stored locally in Chrome.

### Field Mapping

If you use a custom Anki note type, you can choose which Anki field receives each piece of ImmersionKit information.

The important card information is:

* Sentence
* Translation
* Reading
* Screenshot
* Audio

Source information, ID, and URL are optional.

The extension suggests likely mappings automatically, but you can change them.

Multiple pieces of information can also be mapped to the same Anki field. They will be added in order rather than overwriting one another.

## Included Anki Card

The included **ImmersionKit Full Card** note type is designed for sentence recognition.

### Front

The front shows:

* Screenshot
* Japanese sentence
* Sentence audio
* Optional **Furigana** control

### Back

The back keeps the original question visible and adds:

* English meaning
* Optional **Furigana** control
* Smaller screenshot that can be clicked to expand
* Source link
* Collapsible card details

The layout works on desktop and mobile and supports Anki's light and dark modes.

The extension creates **one recognition card per mined sentence** rather than automatically creating multiple card directions.

## Using Your Own Anki Templates

Field mapping controls **where the information is stored**.

Your Anki card template controls **what is actually displayed during review**.

This means mapping information into a field does not automatically make that field appear on an existing custom card template.

The extension does not overwrite customized Anki templates.

## Duplicate Protection

ImmersionKit results are identified using their stable example IDs.

Before adding a card, the extension can check whether that result already exists in Anki.

If it does, the extension opens the existing card instead of creating another copy.

## If Anki Cannot Be Reached

If Anki is closed or AnkiConnect is unavailable, the extension shows:

**Can't reach AnkiConnect. Open Anki, then try again.**

If Anki is running but taking too long to respond, it shows:

**Your Anki is busy right now; try again later.**

## Privacy

The extension runs locally.

It communicates with:

* ImmersionKit to retrieve sentence and media information
* AnkiConnect on your computer to create cards and store media

It does not send your card information to a separate extension server.
