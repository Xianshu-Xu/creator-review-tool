[README.md](https://github.com/user-attachments/files/28031350/README.md)
# Creator Review Tool

Created by Xianshu Xu

Creator Review Tool is a simple browser-based tool for reviewing TikTok creators, posts, and profiles. It helps you quickly approve, reject, skip, tag, and take notes on creators, then export the final results as a CSV file.

## What This Tool Does

- Review TikTok posts grouped by creator
- Review TikTok creator profiles
- Approve, reject, or skip creators with buttons, keyboard shortcuts, or swipe gestures
- Add custom tags such as quality, category, priority, or case-study potential
- Write notes for each creator
- Import data by pasting links or uploading Excel / CSV files
- Auto-save review progress in the browser
- Export progress as a project file
- Export final results as CSV

## How To Start

Open the tool in your browser.

On the home screen, you will see three main setup steps:

1. Choose a review mode
2. Load creator data
3. Set custom tags and project name

After setup, click **Start Review**.

## Review Modes

### 1. Individual Posts

Use this mode when you want to review TikTok posts or videos grouped by creator.

You can load data in three ways:

**Paste Grouped**

Use this when you already have creator IDs and links grouped together.

Format:

```text
7636736562406984000
https://www.tiktok.com/@/video/7636736562406984982
https://www.tiktok.com/@/video/7636421998280723734

7635405708128816000
https://www.tiktok.com/@/video/7635405708128816386
```

Each creator should start with the creator ID, followed by that creator's TikTok links. Leave a blank line between creators.

**Paste Links**

Use this when you only have TikTok post links.

Paste one link per line. The tool will try to group links by username when the username exists in the URL.

**Upload Excel**

Use this when your data is in `.xlsx`, `.xls`, or `.csv` format.

After uploading, choose:

- Creator ID column
- URL column

The tool will group all links under the matching creator ID.

### 2. Creator Profiles

Use this mode when you want to review TikTok profile pages instead of individual posts.

You can load profiles in two ways:

**Paste Profile Links**

Paste one TikTok profile URL per line.

Example:

```text
https://www.tiktok.com/@username1
https://www.tiktok.com/@username2
https://www.tiktok.com/@username3
```

**Upload Excel**

Upload an Excel or CSV file, then select the column that contains the profile URL, handle, or username.

## Custom Tags

Custom tags are optional, but useful if you want more detailed review results.

Each tag has:

- A tag name
- A list of options

Example:

```text
Tag name: Quality
Options: Low, Medium, High
```

During review, the tag options will appear on the right side of the screen. You can click one option for each creator.

If you leave the options field empty, the tool will create a simple **Yes / No** tag.

## Project Name

Give your review a project name before starting.

Example:

```text
UK Shoppable Photos May 2026
```

This name is used when saving progress and exporting files.

## Reviewing Creators

During review, each creator appears as a card.

You can:

- Scroll to see more posts from the same creator
- Add tags on the right panel
- Write notes in the note box
- Approve, reject, skip, or undo decisions

## Keyboard Shortcuts

| Key | Action |
|---|---|
| Right arrow | Approve |
| Left arrow | Reject |
| Up arrow | Skip |
| Z | Undo |
| N | Focus the note box |
| Esc | Finish and go to results |

You can also use the buttons at the bottom of the screen.

## Saving Progress

The tool auto-saves your progress in your browser.

When you come back later using the same browser and device, saved projects will appear under **Resume or Import a Project**.

Important: auto-save is stored locally in your browser. If you change devices, use a different browser, or clear browser data, the saved project may not be available.

## Exporting Progress

While reviewing, click **Export** at the top right to download a project progress file.

This file is useful if you want to:

- Back up your review progress
- Move the project to another device
- Continue later in a different browser

To restore it, use **Import Project File** on the home screen.

## Results Page

When you finish reviewing, the results page shows:

- Number of approved creators
- Number of rejected creators
- Number of skipped creators
- Number of unreviewed creators
- Creators with notes or tags
- Approved creator IDs
- Rejected creator IDs

## Exporting Final Results

Click **Export CSV** to download the final review results.

The CSV includes:

- Creator ID
- Decision
- Custom tag values
- Notes
- Number of posts
- URLs

You can open the CSV in Excel, Google Sheets, or another spreadsheet tool.

You can also copy approved or rejected creator IDs directly with the copy buttons.

## Recommended Workflow

1. Prepare creator links or profile links
2. Open the tool
3. Choose **Individual Posts** or **Creator Profiles**
4. Paste data or upload an Excel / CSV file
5. Add any custom tags you need
6. Enter a project name
7. Click **Start Review**
8. Review each creator
9. Export progress if you want a backup
10. Export CSV when finished

## Notes

- This is a static HTML tool, so it can be hosted on GitHub Pages.
- No server setup is required.
- Review progress is saved locally in the browser.
- TikTok embeds require an internet connection to load properly.

